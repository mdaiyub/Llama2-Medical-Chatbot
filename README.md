# Llama2-Medical-Chatbot

The Llama2 Medical Bot is a powerful tool designed to provide medical information by answering user queries using state-of-the-art language models and vector stores. This README will guide you through the setup and usage of the Llama2 Medical Bot.

## Prerequisites

Before you can start using the Llama2 Medical Bot, make sure you have the following prerequisites installed on your system:

- Python 3.6 or higher
- Required Python packages (you can install them using pip):
    - langchain
    - chainlit
    - sentence-transformers
    - faiss
    - PyPDF2 (for PDF document loading)

## Installation

1. Clone this repository to your local machine.

    ```bash
    git clone https://github.com/mdaiyub/Llama2-Medical-Chatbot.git
    cd Llama2-Medical-Chatbot
    ```

2. Create a Conda virtual environment (optional but recommended):

    ```bash
    conda create -n chatbot python=3.10 -y
    conda activate chatbot
    ```

3. Install the required Python packages:

    ```bash
    pip install -r requirements.txt
    ```

4. Download the required language models and data. Please refer to the Langchain documentation for specific instructions on how to download and set up the language model and vector store. https://huggingface.co/TheBloke/Llama-2-7B-Chat-GGML
Model name: llama-2-7b-chat.ggmlv3.q8_0.bin

5. Set up the necessary paths and configurations in your project, including the `DB_FAISS_PATH` variable and other configurations as per your needs.

6. For the data ingestion and model deployment on the chainlit:
    ```bash
    python ingest.py
    chainlit run model.py -w
    ngrok http 8000 --authtoken 2aALUybQkHSEa9V8W9LpQl6EFmi_7VeHRMStofLaao2YhKuXr
    ```

## Usage

The Llama2 Medical Bot can be used for answering medical-related queries. To use the bot, you can follow these steps:

1. Start the bot by running your application or using the provided Python script.

2. Send a medical-related query to the bot.

3. The bot will provide a response based on the information available in its database.

4. If sources are found, they will be provided alongside the answer.

5. The bot can be customized to return specific information based on the query and context provided.


## License

This project is licensed under the MIT License.

---

For more information on how to use, configure, and extend the Llama2 Medical Bot, please refer to the Langchain documentation or contact the project maintainers.

Happy coding with Llama2 Medical Bot! 🚀



