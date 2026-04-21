# AI Course

AI Course - Instituto Superio Técnico

## Table of contents

- [Python Installation](#python-installation)
- [Python environment](#python-environment)
- [AI Usage](#ai-usage)

### Python Installation

Before starting, make sure you have python installed. If not, follow the instructions below.

#### Windows

1. Download Python from [python.org](https://www.python.org/downloads/) (make sure to install version 3.10 or higher).

2. Install Python (make sure to check "Add Python to PATH" during installation).
   Wait for the installation to finish.

3. Verify the installation by running `python --version` on the terminal.
   The output should be `bash Python 3.10.0` (in the case your version is 3.10, otherwise it will be the version you installed).

   NOTE: If the command is not recognized, it's most likely because Python was not added to the PATH. In that case, you can try to run `py --version` or reinstall Python and make sure to check "Add Python to PATH" during installation.

#### Linux

TODO

#### MacOS

TODO

### Python environment

TL;DR:

```bash
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
```

Python environments are important because they allow you to isolate the dependencies for each project. This means that you can have different versions of the same library installed in different environments without them conflicting with each other. To guarantee that your project is reproducible and does not conflict with other projects, we recommend using a python environment.

1. Start a new python environment:

    ```bash
    python -m venv venv
    ```

    This will create a new folder named `venv` in the current directory. In here, we will install all the dependencies for our project.

2. Activate the python environment:

    ```bash
    venv\Scripts\activate
    ```

    You should see the name of the environment in parentheses at the beginning of the line, like this: `(venv) C:\...\>`. This means that the python environment is activated.

    To leave the environment, run `deactivate`.

3. Install dependencies:

   You can now install dependencies you need for your project using `pip`. For example:

   ```bash
   pip install numpy
   ```

   This will install numpy ONLY inside your environment.

   Dependencies can now be listed in a requirements file by running `pip freeze > requirements.txt`. This will create a file named `requirements.txt` in the current directory that contains all the dependencies you have installed in your environment.

   To install all the dependencies from a requirements file, run `pip install -r requirements.txt`.

4. Check the dependencies you have installed by running `pip list`. It should list all the dependencies you have installed in your environment.

### Getting started

1. Create a new file named `main.py` in the current directory.

2. Open the file in any text editor or IDE. You can use VS Code, PyCharm, or any other IDE.

    NOTE: You can use AI agents to help you write the code, but remember that any AI usage must be reported explicitly in the report.

3. Start with the basic skeleton:

    ```python
    def run():
        pass

    if __name__ == "__main__":
        run()
    ```

4. Save and run the file by running `python main.py` on the terminal.

### AI Usage

This AI Course is classified as **Level 1 (Yellow)**, which means that the usage of AI tools is allowed, but must be reported explicitly in the report.

At this level, the use of AI tools is permitted for tasks within an assessment component, such as idea generation, topic organisation, brainstorming, linguistic review, structure suggestions, summarising, among others. Any generated content that is included in the final work must be reviewed and edited, so a Declaration of Use and of the purpose of that use is required, including, if requested by lecturers, the prompts used.

**Declaration of Use Template:**
"All decisions and technical content in this work are of my own authorship.
[List tools] were used for [functions]"

**Example:**
"All decisions and technical content in this work are of my own authorship. ChatGPT by OpenAI (2025) [https://chat.openai.com] was used to generate the table of contents of the work."
