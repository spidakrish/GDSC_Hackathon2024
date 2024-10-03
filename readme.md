
# GPT-3.5 Terminal Chatbot

This repository contains a simple terminal-based chatbot powered by OpenAI's GPT-3.5. The assistant can respond to a variety of user inputs and provide helpful information based on natural language queries.

## Features

- Interact with OpenAI's GPT-3.5 model directly from the terminal.
- Conversational AI that can handle various questions and requests.
- Easy-to-use command-line interface.
- Ability to exit the chatbot by typing "exit" or "quit."

## Prerequisites

Before you begin, ensure you have the following installed:

- Python 3.7 or later.
- An OpenAI API key. You can sign up for an API key [here](https://beta.openai.com/signup/).

## Installation

1. **Clone this repository**:

    ```bash
    git clone https://github.com/yourusername/gpt-terminal-chatbot.git
    cd gpt-terminal-chatbot
    ```

2. **Create a virtual environment (optional but recommended)**:

    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use: venv\Scripts\activate
    ```

3. **Install dependencies**:

    You only need the `openai` library, which can be installed via pip:

    ```bash
    pip install openai
    ```

4. **Set up your OpenAI API key**:

    Create a `.env` file in the root directory of the project and add your OpenAI API key. This keeps your API key secure and avoids hardcoding it into your scripts.

    **Example `.env` file**:
    ```text
    OPENAI_API_KEY=your-api-key-here
    ```

    Alternatively, you can export the API key as an environment variable directly in your shell:

    ```bash
    export OPENAI_API_KEY=your-api-key-here
    ```

## Usage

To start the chatbot, simply run the script:

```bash
python google.py
```

### Example Interaction

```
Welcome to your GPT-powered assistant in the terminal!
You: What's the capital of Australia?
GPT: The capital of Australia is Canberra.

You: exit
Exiting the assistant. Goodbye!
```

### Commands

- **Normal Chat**: Just type your questions or statements, and the chatbot will respond.
- **Exit**: Type `exit` or `quit` to close the program.

## Project Structure

```
.
├── google.py          # Main script that runs the chatbot
├── README.md          # Project documentation (this file)
├── .env.example       # Example of how to structure your environment file
└── .gitignore         # Ignore Python cache and environment variables
```

## Environment Variables

Ensure your `.env` file contains the following:

```text
OPENAI_API_KEY=your-api-key-here
```

This key is necessary to authenticate your requests to the OpenAI API. Do **not** share your API key publicly or commit it to Git.

## Best Practices for API Security

- **Do not** hard-code API keys directly in the code. Use environment variables instead.
- **Add a `.gitignore`** file to exclude sensitive files like `.env` from being tracked by git. Here's an example `.gitignore`:

    ```text
    # Python cache files
    __pycache__/
    *.py[cod]

    # Environment variables
    .env
    ```

## Future Enhancements

- Add support for switching between different GPT models (e.g., GPT-3.5 and GPT-4).
- Implement error logging for better troubleshooting.
- Add a web interface using Flask or Django for more user-friendly interaction.
- Improve handling of different input formats, like voice commands or file uploads.

## Contributing

If you wish to contribute to the project, feel free to submit a pull request or open an issue. Contributions, bug reports, and feature requests are welcome.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgements

This project uses OpenAI's API to power the chatbot. Special thanks to the developers at OpenAI for their work in advancing AI technology.
