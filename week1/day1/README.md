# Days 1

This project is a small Python starter for working with Groq-powered LLM APIs. It includes a basic "Hello World" script and a sample script that sends a prompt to a Groq model and prints the model response.

## Project overview

- `main.py` — simple Python entry point that prints a greeting.
- `hellollm.py` — connects to Groq using the `groq` SDK and makes a chat completion request.
- `pyproject.toml` — project metadata and Python dependencies.

## Prerequisites

- Python 3.14 or newer
- A Groq API key

## Setup

1. Open a terminal in this project folder.
2. Create and activate a virtual environment:

   ```bash
   python -m venv .venv
   .venv\Scripts\activate
   ```

3. Install the project dependencies:

   ```bash
   pip install groq python-dotenv
   ```

   Or, if you use `uv`:

   ```bash
   uv sync
   ```

4. Create a `.env` file in the project root with your Groq API key:

   ```env
   GROQ_API_KEY=your_api_key_here
   ```

## Run the project

Run the basic app:

```bash
python main.py
```

Run the Groq API example:

```bash
python hellollm.py
```

## Example output

The Groq example sends a prompt such as "do you know who is virat kohli" and prints the model response returned by the API.

## Notes

- The project uses the `python-dotenv` package to load environment variables from `.env`.
- The model used in the sample is `openai/gpt-oss-120b`.
- Make sure your Groq API key is kept private and not committed to version control.

## License

This project is for learning and experimentation purposes.
