# Orange Agent

This project contains a script for creating an interactive generative agent, leveraging the power of OpenAI's GPT-3.5-turbo model.

## Description

The script `orange_agent.py` comprises three main components:

1. `ChatBot`: A simple interface to OpenAI's GPT-3.5-turbo model. It takes a user's message as input and returns a generated response.

2. `MemoryStore`: Manages the memory of the generative agent, providing functionality to save, load, and search for relevant memories. Memories are saved as strings and searched using TF-IDF vectorization and cosine similarity.

3. `GenerativeAgent`: Represents a generative agent that uses both the `ChatBot` and `MemoryStore` classes. The agent generates responses to user input, learns from interactions by storing them in memory, and can provide a summary of its state.

## Usage

The script ends with some sample interactions with an instance of the `GenerativeAgent` class. The agent is created, given some memories, asked to generate responses, aged by a few years, and finally asked to provide a summary of its state.

Run the script with `python orange_agent.py` and interact with the generative agent via the console.

## Requirements

The script requires the following Python packages:
- `sqlite3`
- `sklearn`
- `os`
- `pickle`
- `openai`

Install them with `pip install -r requirements.txt`.
