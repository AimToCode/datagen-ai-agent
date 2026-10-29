# DataGen AI Agent

A beginner learning project: a Python command-line AI agent that generates fake sample users, saves them as JSON, and answers questions by reading the saved data.

## Features

- Generate sample users with names, email domains, and an age range.
- Save generated users to JSON files in the `data/` folder.
- Read saved JSON files and answer questions about their contents.
- Uses Python tools that the AI agent can choose when needed.

## Built with

- Python
- uv
- LangChain
- LangGraph
- OpenAI API

## Requirements

- Python
- uv
- An OpenAI API key

## Setup

1. Clone this repository and open its folder in a terminal.
2. Install the project dependencies:

   ```powershell
   uv sync
   ```

3. Create a file named `.env` in the project root, next to `pyproject.toml`.
4. Add your OpenAI API key to `.env`:

   ```text
   OPENAI_API_KEY=your_key_here
   ```

   Replace `your_key_here` with your key. Keep `.env` private and never commit it to GitHub.

5. Start the agent:

   ```powershell
   uv run python main.py
   ```

## Example prompts

```text
Generate users named Asha, Kabir, and Maya, use company.com emails, age 25 to 35, and save them as users.json.
```

```text
Who is the oldest user in users.json?
```

The agent saves and reads files under `data/`. Type `quit` to exit.

## Notes

This is a learning prototype for working with AI agents and Python tools. The generated users are fictional sample data, not real people. OpenAI API usage may incur charges.
