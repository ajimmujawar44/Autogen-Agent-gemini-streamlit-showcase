# AutoGen Gemini Agent Demos

A collection of Streamlit demos exploring Microsoft AutoGen agents with Google's Gemini API. The examples cover single-agent Q&A, multi-agent collaboration and planning, and image analysis.

## Demos

- `ag_single_agent.py` — a single-agent mentor for non-technical questions.
- `ag_multiagent.py` — Analyst, Developer, and Reviewer collaboration on a task.
- `AG_Multiagent01.py` — coordinated school and office planning with three agents.
- `ag_father.py` — another multi-agent morning-planning example.
- `ag_multimsg.py` — image-question answering with Gemini vision.
- `ag_gemini.py` — a command-line Gemini and AutoGen connectivity example.
- `autogen_testing.py` — a small AutoGen API test.

## Screenshots

The `screenshots/` folder contains example captures of the Streamlit demos and their outputs.

## Setup

Use Python 3.11 or newer. From the project directory, create and activate a virtual environment, then install the dependencies:

```powershell
py -3.11 -m venv .venv
.\.venv\Scripts\Activate.ps1
python -m pip install -r requirements.txt
```

Create a local `.env` file from `.env.example` and set your Gemini API key:

```text
GEMINI_API_KEY=your-real-api-key
```

Never commit `.env` or publish API keys. The `.gitignore` excludes local environment files and virtual environments.

## Run a Streamlit demo

For example:

```powershell
streamlit run ag_multiagent.py
```

Run another demo by replacing the filename with one of the Streamlit scripts above. The command-line example can be run with:

```powershell
python ag_gemini.py
```

Gemini API usage is subject to the quota and billing limits for your Google AI Studio project.
