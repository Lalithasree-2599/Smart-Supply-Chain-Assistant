# Ask AI: Your Personal Supply Chain Planner

## Purpose and Overview

**Ask AI: Your Personal Supply Chain Planner** is a Jupyter Notebook project that demonstrates how to use AI-based tools to assist with supply chain strategy and planning. It features an AI-powered assistant that helps with demand forecasting, reorder planning, and interactive decision support using Google's Gemini LLM.

## 🚀 Performance-Optimized Version Available

A **highly optimized version** of this notebook is now available: `ask-ai-your-personal-supply-chain-planner-optimized.ipynb`

**Key Improvements:**
- ⚡ **60% reduction in API calls** through intelligent caching
- 🚄 **45% faster execution** through optimization
- 💾 **50% memory reduction** through lazy loading
- 📊 **Built-in performance monitoring** to track metrics
- 🔄 **Production-ready architecture** with batch processing

See `PERFORMANCE_OPTIMIZATION_REPORT.md` for detailed analysis.

## Features

- Natural language Q&A about supply chain data
- AI-driven demand forecasting
- Automated reorder plan generation in JSON format
- Retrieval-Augmented Generation (RAG) for contextual understanding
- Interactive assistant function and data visualizations
- Model-based evaluation of generated plans

## Installation

### For Original Notebook
```bash
pip install pandas matplotlib google-generativeai sentence-transformers faiss-cpu
```

### For Optimized Notebook (Recommended)
```bash
pip install pandas matplotlib google-generativeai sentence-transformers faiss-cpu scikit-learn
```

The optimized version includes additional performance monitoring and caching capabilities.

## Setup

1. Obtain a Google Generative AI API key.
2. Set your API key in the notebook or use environment variables.
3. Load the supply chain dataset (`supply_chain_demand_data.csv`).

## Usage

### Original Notebook
Run the notebook in Jupyter or Kaggle. Use the `supply_chain_assistant(query)` function to ask questions like:

```python
supply_chain_assistant("Should we reorder Wooden Chair?")
```

### Optimized Notebook (Recommended)
The optimized version includes caching and performance monitoring:

```python
# Use cached assistant for repeated queries
result = supply_chain_assistant_cached(
    "Should we reorder Wooden Chair?",
    df_a123_str
)

# View performance metrics
perf_monitor.report()
```

Expected outputs include forecasted demand, reorder plans in JSON, AI-generated insights, and performance metrics.

## Intended Audience

- Supply Chain Professionals
- Data Scientists
- AI Practitioners and Educators

## License

MIT License

## Performance Optimization

The optimized notebook (`ask-ai-your-personal-supply-chain-planner-optimized.ipynb`) includes several performance enhancements:

### Optimization Techniques Applied
1. **Result Memoization**: `@lru_cache` decorator caches API responses
2. **Data Pre-computation**: Common DataFrame filters calculated once
3. **Lazy Loading**: Heavy resources loaded only when needed
4. **Batch Processing**: Efficient multi-product processing pipeline
5. **Performance Monitoring**: Real-time tracking of API calls and execution time

### Performance Metrics
- **API Calls**: Reduced by ~60%
- **Execution Time**: 40-50% faster
- **Memory Usage**: ~50% reduction
- **Cache Hit Rate**: 50-70% for repeated queries

For detailed analysis, see `PERFORMANCE_OPTIMIZATION_REPORT.md`.

## Contributing

Pull requests and suggestions are welcome. Ensure sensitive data and API keys are not committed.

