# Data Science & AI Intern Assignments

This repository serves as a template for assignments throughout the internship program. Interns should create their own repository from this template and use it to organize all weekly assignments.

## Getting Started

1. Click the "Use this template" button at the top of this GitHub repository
2. Name the new repository `ds-ai-assignments-[user-name]` (e.g., `ds-ai-assignments-john-doe`)
3. Make the new repository private
4. Share access with assigned mentor(s)
5. Clone the new repository to a local machine

## How to Use

### Prerequisites

- Python 3.12+
- Poetry for dependency management

### Install Python

Ensure you have Python 3.12 installed. You can download it from the [official website](https://www.python.org/downloads/).

### Install Poetry

Install Poetry by running:

```bash
# For Unix/Linux/OS X/wsl
curl -sSL https://install.python-poetry.org | python3 -

# For Windows (PowerShell)
(Invoke-WebRequest -Uri https://install.python-poetry.org -UseBasicParsing).Content | python -

```
For more details, visit the [Poetry documentation](https://python-poetry.org/docs/#installation).

### Set Up the Virtual Environment

To create a virtual environment using Python 3.12, run:

```
poetry env use 3.12
```

### Install Dependencies

Install all project dependencies, including development tools:

```bash
poetry install
```
### Install additional packages as needed:

```bash
poetry add package-name
```

## Code Quality Tools

This template includes several code quality tools to help write clean, consistent code:

* `Black`: Automatic code formatter
* `isort`: Import organizer
* `Ruff`: Fast Python linter

These tools are configured in `pyproject.toml` with a line length of 120 characters.

### How to Use the Tools

* Black
Format your code:

```
poetry run black .
```

isort
Sort your imports:

```
poetry run isort .
```

Ruff
Analyze your code for linting errors:

```
poetry run ruff check .
```

## Repository Structure

This repository is organized by weeks, with a separate folder for each week's assignments:
```
├── weeks/
│   ├── ...
│   ├── week7/  # RAG & AI Agents
│   └── ...
└── capstone/  # Final project
```

For each week of the program:

1. Receive the week's learning materials and assignment instructions from mentors
2. Work in the corresponding week's folder in this repository
3. Create the following components in the week's folder (when needed):
    * notebooks/ : Jupyter notebooks for exploration and analysis
    * src/ : Python modules and scripts
    * data/ : Data files or scripts to load data
3. Commit work regularly with descriptive commit messages
4. Push to GitHub repository
5. Notify mentor when complete

## Assignment Structure Guidelines

Each week's assignment should typically include:

1. A clear `Report` documenting:
    * The approach taken
    * Key findings and results
    * Any challenges encountered and how they were addressed
    * Instructions for running the code
2. Well-organized code:
    * Document functions and classes
    * Separate code into modules where appropriate
3. Notebooks for exploration:
    * Include markdown cells to explain reasoning
    * Keep outputs in the notebook
    * Clean up exploration work before submission
