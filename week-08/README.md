# Amazon Annual Report Assistant

A retrieval-augmented question-answering assistant that uses Amazon's 2024 and 2025 annual reports to answer business and financial questions with supporting evidence.

**Built with:** Python · FAISS · Sentence Transformers · Gemini · PyPDF

## How It Works

- **Retrieve:** FAISS searches annual-report passages embedded with `all-MiniLM-L6-v2`.
- **Guide:** Dynamic few-shot prompting selects relevant examples to help shape responses.
- **Calculate:** A calculator tool handles arithmetic when given an expression.
- **Generate:** Gemini produces answers using retrieved evidence and examples.
- **Evaluate:** Component metrics and an LLM judge to assess system performance.

These techniques bring together document retrieval, example-based prompting, tool use, and answer evaluation in one application.

## Results

| Evaluation metric | Result |
|---|---:|
| Routing accuracy | 90% |
| Retrieval evidence match rate | 80% |
| Calculator accuracy | 100% |
| LLM judge — correctness | 4.40/5 |
| LLM judge — grounding | 4.60/5 |
| LLM judge — citation quality | 4.60/5 |

The LLM judge evaluated 10 held-out questions. These results are an initial assessment, not a guarantee of answer quality.

## What I Learned

Testing revealed two main weaknesses:

- **Retrieval relevance:** Indirect questions sometimes retrieved less relevant passages than more specific questions.
- **Tool selection:** The assistant sometimes routed calculation questions to RAG instead of the calculator, even when the retrieved evidence contained the necessary numbers.

Potential improvements include better tool routing, retrieval reranking, and a larger evaluation set with manually verified answers.

## Run the Project

Open [`week8_capstone.ipynb`](week8_capstone.ipynb) and run the notebook in order.

The notebook expects these files in your Google Drive under `/content/drive/MyDrive/Datasets/`:

- `Amazon-2024-Annual-Report.pdf`
- `Amazon-2025-Annual-Report.pdf`

A valid `GEMINI_API_KEY` is required for Gemini-based generation and evaluation.
