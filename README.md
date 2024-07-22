# MENTORIA helper pipeline

This project leverages the crewAI framework to generate high-quality documentation for the [**MENTORIA**](https://github.com/mohamedhassan218/mentoria-demo), a Retrieval Augmented Generation (RAG) tool designed to enable users to chat with their data from various sources such as PDFs, Word documents, text files, and URLs.

## Overview

The MENTORIA Multi-Agent Documentation Pipeline is an innovative approach to creating comprehensive and accurate documentation using a multi-agent system. The pipeline involves three key agents:

1. **Content Planner**
2. **Content Writer**
3. **Editor**

Each agent plays a crucial role in ensuring that the final documentation is well-structured, insightful, and polished.

## Agents and Tasks

### Content Planner

- **Role:** Plan engaging and factually accurate content on the given topic.
- **Backstory:** Responsible for planning documentation, collecting relevant information, and laying the foundation for the Content Writer.

### Content Writer

- **Role:** Write insightful and factually accurate documentation on the given topic.
- **Backstory:** Tasked with writing new documentation based on the Content Planner's outline and context, following main objectives, and providing objective insights.

### Editor

- **Role:** Edit the documentation for clarity, grammar, and alignment with the brand's voice.
- **Backstory:** Responsible for editing the documentation, ensuring clarity, grammatical correctness, and brand voice alignment.

## Tasks

### Plan Task
The Content Planner identifies the latest trends, key players, and noteworthy news on the topic, defines the target audience, develops a detailed content outline, and includes SEO keywords and relevant sources.

### Write Task
The Content Writer uses the content plan to craft a compelling chapter on the topic, incorporates SEO keywords naturally, names sections/subtitles engagingly, structures the content with an engaging introduction, insightful body, and summarizing conclusion, and proofreads for grammatical errors and brand voice alignment.

### Edit Task
The Editor proofreads the documentation for grammatical errors and alignment with the brand's voice, ensuring it is ready for publication.

## Usage

To use this pipeline, follow these steps:

1. Clone this repository:
    ```bash
    git clone git@github.com:mohamedhassan218/mentoria-helper.git
    ```

2. Create a virtual environment:
    ```bash
    python -m venv .venv
    ```

3. Activate your virtual environment:
    - On Windows:
        ```bash
        .venv\Scripts\activate
        ```

    - On Unix or MacOS:
        ```bash
        source .venv/bin/activate
        ```

4. Install the dependencies:
    ``` bash
    pip install -r requirements.txt
    ```

5. Create a `.env` file in the project root and add the following environment variables:
    ```
    GOOGLE_API_KEY=""
    SERPER_API_KEY=""
    ```
    - Get your free **Google** API key from [here](https://ai.google.dev/gemini-api/docs/api-key)
    - Get your free **Serper** API key from [here](https://serper.dev/api-key)



## Showcase

This simple pipeline is a testament to the power of Generative AI agents working together to produce high-quality content. This innovative approach ensures that documentation is not only informative but also engaging and well-structured, making it an invaluable tool for both developers and users of the MENTORIA application.


## Contributing

Contributions are welcome! If you have any ideas, suggestions, or improvements, please feel free to open an issue or submit a pull request.