# LLM-Number-Convergence-Study
Investigating Cognitive Biases and Convergence Patterns in Large Language Models' Pseudo-Random Number Selection

# LLM Number Convergence Study

An empirical study investigating convergence patterns in Large Language Models' pseudo-random number selection.

## Overview

This experiment tests whether different Large Language Models exhibit convergent behavior when asked to select "random" numbers, potentially revealing shared cognitive biases inherited from their training data.

### Key Finding
When asked to "pick a number between 1 and 50", multiple state-of-the-art LLMs (GPT-4, Claude, Gemini, Llama, Mistral) showed a significant preference for the number **27**.

## Research Question

Do different LLMs trained on similar datasets exhibit convergent cognitive biases in pseudo-random number selection?

## Quick Start

### Prerequisites

- Python 3.8+
- Jupyter Notebook
- OpenRouter API key

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/llm-number-convergence-study.git
cd llm-number-convergence-study
```

2. Install dependencies:
```bash
pip install openai pandas matplotlib seaborn numpy scipy jupyter
```

3. Set your OpenRouter API key in the notebook:
```python
OPENROUTER_API_KEY = "your-api-key-here"
```

4. Run the experiment:
```bash
jupyter notebook llm_number_convergence_experiment.ipynb
```

## Experiment Design

### Models Tested
- OpenAI GPT-4 (gpt-4o)
- Anthropic Claude 3.5 (claude-3.5-sonnet)
- Google Gemini 2.0 (gemini-2.0-flash-exp)
- Meta Llama 3.1 (llama-3.1-70b-instruct)
- Mistral Large (mistral-large)

### Test Parameters
- **Number Ranges**: (1,10), (1,50), (1,100), (0,9), (1,1000)
- **Prompt Variants**: 6 different formulations
- **Temperature**: 0.7
- **Iterations**: 10-20 per test condition

## Output Files

The experiment generates:
- `llm_number_convergence_results.json` - Complete experiment data
- `llm_number_selections.csv` - Raw selection data
- `llm_convergence_dashboard.png` - Visual summary dashboard

## Key Results

- **Convergence Points**: Models show statistically significant preference for certain numbers
- **Cognitive Biases**: LLMs exhibit human-like biases (prime preference, avoiding extremes)
- **Cross-Model Similarity**: High correlation in selection patterns across different models

## License

MIT
