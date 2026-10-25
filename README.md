![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# Lab | Agents and Tools


## Introduction

A bank's product team spends hours answering the same kind of questions: how many customers are on the Premium plan, what the competition charges, how many complaints were about card delivery. Some answers are in the bank's internal documents, some are on the web, and many need a quick calculation. In this lab you build a research assistant with LangChain: an agent with a calculator of your own, a retrieval tool over the bank's documents, and web search with Tavily, which cites where every fact came from. You trim long search results to control the cost, evaluate on eight questions whether the agent chooses the right tools and what each answer costs, give it memory, and stop it with a step limit. In the extra task, the assistant listens to a spoken question and answers out loud.

The lab follows the **Agents and Tools** lesson step by step.


## Getting Started

Open the `main.ipynb` file in the `your-code` directory. Follow the instructions, add your code, and answer the questions in the markdown cells. Each challenge ends with a checkpoint that tells you what you should see. The documents are in the `data` folder: `bank_documents.csv` has ten short internal documents of the bank, with the columns `id`, `title` and `text`.

The lab needs `pip install openai python-dotenv langchain langchain-openai langchain-tavily sentence-transformers chromadb tiktoken`, the OpenAI API key that Ironhack gives you, and a free Tavily API key from [tavily.com](https://www.tavily.com) (no card needed). Create a file called `.env` in the `your-code` folder with two lines, `OPENAI_API_KEY=sk-...` and `TAVILY_API_KEY=tvly-...`. The repository's `.gitignore` already excludes `.env`: **never write your keys in the notebook, and run `git status` before every commit to check that `.env` is not listed.** The whole lab costs about one US cent and fewer than 20 Tavily searches.

## Deliverables

- `main.ipynb` with your code, its outputs, and your answers.

## Submission

Upon completion, add your deliverables to git. Then commit git and push your branch to the remote.

## Resources

- [LangChain documentation: agents](https://docs.langchain.com/oss/python/langchain/agents)
- [LangChain documentation: tools](https://docs.langchain.com/oss/python/langchain/tools)
- [Tavily documentation](https://docs.tavily.com/)
- [Chroma documentation](https://docs.trychroma.com/)

## Data

`data/bank_documents.csv` was written for this course: the bank, its products and its numbers are invented.
