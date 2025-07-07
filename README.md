# self_awareness_evals

This project is a codebase for evaluating self-awareness in AI models. It includes implementations for interacting with OpenAI and Anthropic APIs to generate responses, as well as utilities for retrying API calls with exponential backoff to handle rate limits.

## Features

- Integration with OpenAI and Anthropic language models.
- Functions to generate responses from these models with configurable parameters.
- Retry mechanism with exponential backoff for robust API interaction.
- Helper functions for formatting multiple-choice questions for AI prompts.
- Example usage of generating responses to multiple-choice questions.

## Installation

The project requires Python and the following dependencies:

- openai (>=1.56.1)
- anthropic
- inspect_ai
- tabulate
- wikipedia
- jaxtyping
- python-dotenv
- httpx
- pandas
- tqdm

You can install the dependencies using pip:

```bash
pip install openai>=1.56.1 anthropic inspect_ai tabulate wikipedia jaxtyping python-dotenv httpx pandas tqdm
```

## Setup

1. Set your OpenAI and Anthropic API keys in environment variables:

```bash
export OPENAI_API_KEY="your_openai_api_key"
export ANTHROPIC_API_KEY="your_anthropic_api_key"
```

2. Alternatively, create a `.env` file with the following content:

```
OPENAI_API_KEY=your_openai_api_key
ANTHROPIC_API_KEY=your_anthropic_api_key
```

## Usage

- The main function `generate_response_basic` allows generating responses from specified models with options for temperature, max tokens, and stop sequences.
- The `retry_with_exponential_backoff` decorator wraps the response generation function to handle rate limits gracefully.
- Helper functions assist in formatting prompts for multiple-choice questions.
- Example multiple-choice questions are included in the codebase to demonstrate usage.

## Author

Tommy Xie (TommyXie_@outlook.com)

## Source Credit

ARENA 3.0
