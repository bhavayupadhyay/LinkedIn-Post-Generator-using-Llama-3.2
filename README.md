# Project: GenAI Post Generator

This tool analyzes the posts of a LinkedIn influencer and helps them create new posts that match their writing style.

<img src="resources/tool.jpg" alt="Tool Illustration" />

## Overview

Let's say Mohan is a LinkedIn influencer who needs help writing future posts. This tool allows him to upload his past LinkedIn posts for analysis. It extracts key topics, allowing him to select the topic, length, language, etc., and then generates a new post that aligns with his existing writing style.

## Technical Architecture

<img src="resources/architecture.jpg" alt="Technical Architecture" />

1. **Stage 1**: Collect LinkedIn posts and extract key attributes such as Topic, Language, and Length.
2. **Stage 2**: Use the extracted attributes (topic, language, length) to generate a new post. Past posts related to the selected topic, language, and length are used for few-shot learning to guide the large language model (LLM) in replicating the writing style.

## Setup

Follow these steps to set up and run the project:

1. Obtain an API key:
   - Get your API_KEY from [Groq Console](https://console.groq.com/keys).
   - Update the `.env` file by adding your API key as `GROQ_API_KEY`.

2. Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the Streamlit app:
    ```bash
    streamlit run main.py
    ```

## License

This software is licensed under the MIT License. However:

- **Commercial use is strictly prohibited** without prior written permission from the author.
- Attribution must be provided in all copies or substantial portions of the software.

---

Copyright (C) Codebasics Inc. All rights reserved.
