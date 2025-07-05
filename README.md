# Mystery Em Dash Analysis

This repository contains analysis and research on em dash usage patterns in AI-generated text across different language models.

The detailed description of the study is found in the substack blog:

https://msukhareva.substack.com/p/the-mystery-of-emdashes-part-two

## Project Structure

```
├── analysis_results_substack/     # Analysis results and visualizations
│   ├── images/                    # Generated charts and graphs
│   ├── paraphrase_results_*.json  # Paraphrase analysis data
│   └── story_analyses_*.json      # Story analysis data
└── notebooks/                     # Jupyter notebooks for analysis
    └── pipeline_data_generation.ipynb
```

## Overview

This project investigates how different AI language models (GPT-3.5 Turbo, GPT-4o, GPT-4.1) use em dashes in generated text, including:

- Em dash frequency analysis across models
- Token distribution changes when paraphrasing sentences with em dashes
- Statistical comparison of em dash usage patterns
- Visualization of model-specific behavior

## Data Analysis

The analysis includes:
- **Story Generation**: Analysis of em dash usage in originally generated stories
- **Paraphrasing**: Token difference analysis when paraphrasing sentences containing em dashes
- **Model Comparison**: Statistical comparison across different AI models
- **Visualization**: Custom charts showing usage patterns and distributions

## Files

- `analysis_results_substack/`: Contains JSON data files with analysis results
- `notebooks/`: Jupyter notebooks for data processing and analysis
- Generated visualizations are saved in `analysis_results_substack/images/`

## Setup

### Prerequisites
- Python 3.x
- Jupyter Notebook
- Azure OpenAI API access

### Environment Configuration
1. Copy `.env.template` to `.env`
2. Fill in your Azure OpenAI credentials in the `.env` file:
   ```
   AZURE_OPENAI_API_KEY=your-actual-api-key
   AZURE_OPENAI_API_VERSION=2025-01-01-preview
   AZURE_OPENAI_ENDPOINT=https://your-endpoint.openai.azure.com
   ```
3. The `.env` file is ignored by git for security

### Installation
```bash
pip install openai python-dotenv tiktoken pandas matplotlib seaborn
```

## Usage

1. Run the notebooks in the `notebooks/` directory
2. Analysis results and visualizations will be generated in `analysis_results_substack/`
3. View the generated charts in the `images/` subfolder

## Requirements

- Python 3.x
- Jupyter Notebook
- pandas, matplotlib, seaborn
- JSON processing libraries

---

*Research into AI language model behavior and text generation patterns.*
