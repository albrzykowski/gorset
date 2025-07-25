# Prompt Compressor

A browser-based tool for compressing natural language prompts by leveraging a large language model (LLM) via OpenAI's API. Users can interactively apply specific compression strategies—such as synonym replacement, semantic compression, or generalization—while preserving the original meaning. The tool compares input and output by character and token count, and visually highlights differences.

## Features

- Prompt compression using GPT-based models
- Optional compression strategies via checkboxes:
  - **Use shorter synonyms** – Replace words or phrases with more concise synonyms without altering meaning.
  - **Paraphrase while preserving structure** – Rewrite sentences using simpler wording while keeping the original logical or syntactic structure.
  - **Remove non-essential information** – Eliminate phrases or elements that are redundant or contribute little to the prompt’s intent.
  - **Generalize details** – Replace specific examples or terminology with broader, more abstract equivalents.
  - **Compress semantically** – Perform high-level semantic compression, minimizing token usage while retaining intent and constraints.
- Token and character comparison (with percentage difference)
- Visual diff highlighting:
  - Red: removed elements
  - Green: added elements
  - Yellow: modified phrases
- Client-side only; no data is stored or sent beyond OpenAI API

## Requirements

- A valid **OpenAI API token**
- Internet connection
- Modern browser with JavaScript enabled

## Usage

1. Open `index.html` in your browser.
2. Enter your OpenAI API key when prompted (stored in session memory only).
3. Paste your prompt in the text area.
4. Select desired compression options via checkboxes:
   - Use shorter synonyms
   - Paraphrase while preserving structure
   - Remove non-essential information
   - Generalize details
   - Compress semantically
5. Click **Compress Prompt** to generate output.
6. View the compressed version, token statistics, and highlighted differences.

## Disclaimer

This tool uses the OpenAI API in real time. All API usage costs are incurred by the user. Ensure compliance with OpenAI’s usage terms and your organization’s data handling requirements.

## License

MIT License
