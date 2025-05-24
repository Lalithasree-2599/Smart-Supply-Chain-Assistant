# Ask AI: Your Personal Supply Chain Planner

## Purpose and Overview

**Ask AI: Your Personal Supply Chain Planner** is a Jupyter Notebook project that demonstrates how to use AI-based tools to assist with supply chain strategy and planning. It features an AI-powered assistant that helps with demand forecasting, reorder planning, and interactive decision support using Google's Gemini LLM.

## Features

- Natural language Q&A about supply chain data
- AI-driven demand forecasting
- Automated reorder plan generation in JSON format
- Retrieval-Augmented Generation (RAG) for contextual understanding
- Interactive assistant function and data visualizations
- Model-based evaluation of generated plans

## Installation

```bash
pip install pandas matplotlib google-generativeai sentence-transformers faiss-cpu
```

## Setup

1. Obtain a Google Generative AI API key.
2. Set your API key in the notebook or use environment variables.
3. Load the supply chain dataset (`supply_chain_demand_data.csv`).

## Usage

Run the notebook in Jupyter or Kaggle. Use the `supply_chain_assistant(query)` function to ask questions like:

```python
supply_chain_assistant("Should we reorder Wooden Chair?")
```

Expected outputs include forecasted demand, reorder plans in JSON, and AI-generated insights.

## Intended Audience

- Supply Chain Professionals
- Data Scientists
- AI Practitioners and Educators

## License

MIT License

## Contributing

Pull requests and suggestions are welcome. Ensure sensitive data and API keys are not committed.

