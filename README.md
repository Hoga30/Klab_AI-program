# AI and Machine Learning projects at Klab

# Day 1 — Python for AI

This project contains my Day 1 Python for AI assignment. It includes Python practice, a Jupyter notebook, project dependencies, a smoke test, and a chart created using Matplotlib.

## Project Structure

```text
klab-Ai-Rose/
│
├── notebooks/
│   └── day01_python_for_ai.ipynb
│
├── reports/
│   └── day01_chart.png
│
├── src/
│
├── .env.example
├── .gitignore
├── README.md
└── requirements.txt
```

## Requirements

Before starting, make sure Python is installed on your computer.

You can check your Python installation with:

```bash
python --version
```

## Setup and Reproduction

Follow these steps to reproduce the assignment from a fresh copy of the repository.

### 1. Create the virtual environment

Open a terminal in the project folder and run:

```bash
python -m venv .venv
```

This creates a virtual environment named `.venv`.

### 2. Activate the virtual environment

On Windows, run:

```bash
.venv\Scripts\activate
```

When the environment is activated, you should see `(.venv)` at the beginning of your terminal prompt.

### 3. Install the dependencies

With the virtual environment activated, install the required Python packages:

```bash
pip install -r requirements.txt
```

This installs the dependencies needed to run the assignment.

### 4. Run the smoke test

Run:

```bash
python -m pytest -q
```

The smoke test checks that the project is working correctly.

If the test passes, continue to the notebook.

### 5. Open the assignment notebook

Open the following file in VS Code:

```text
notebooks/day01_python_for_ai.ipynb
```

Select the project's `.venv` Python environment as the notebook kernel.

Then run the notebook from the first cell to the last cell.

## Notebook

The notebook contains the Python for AI exercises completed for Day 1.

The notebook should run successfully after restarting the kernel and using **Run All**.

## Generated Report

The notebook generates a chart showing how scores change across four attempts.

The chart is saved as:

```text
reports/day01_chart.png
```

The chart demonstrates that the score improves significantly during the first three attempts and then begins to plateau.

## Environment Variables

The `.env.example` file is provided as a template for environment variables if they are required later.

It does not contain real passwords, API keys, or other secrets.

## Important Notes

* Do not commit the `.venv/` folder to Git.
* Do not commit passwords, API keys, or other secrets.
* Use `.env.example` as a template for required environment variables.
* Run the notebook from beginning to end to verify that all cells execute without errors.
