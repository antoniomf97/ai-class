# AI Course

AI Course - Instituto Superio Técnico

## Table of contents

- [Python Installation](#python-installation)
- [Python environment](#python-environment)
- [AI Usage](#ai-usage)

### Python Installation

Before starting, make sure you have python installed. If not, follow the instructions below.

#### Windows

1. Open a terminal and run the following command to check if Python is already installed:
   `python --version`.
   If Python 3.10 or higher is already installed, you can skip the steps below.

2. Download Python from [python.org](https://www.python.org/downloads/) (make sure to install version 3.10 or higher).

3. Install Python (make sure to check "Add Python to PATH" during installation).
   Wait for the installation to finish.

4. Verify the installation by running `python --version` on the terminal.
   The output should be `bash Python 3.10.0` (or whichever version was installed).

   > **Note:** If the command is not recognized, it's most likely because Python was not added to the PATH. In that case, you can try to run `py --version` or reinstall Python and make sure to check "Add Python to PATH" during installation.

#### Linux

1. Open a terminal and run the following command to check if Python is already installed:
   `python3 --version`.
   If Python 3.10 or higher is already installed, you can skip the steps below.

2. Update your package list and install Python:

    ```bash
    sudo apt update
    sudo apt install python3 python3-pip
    ```

   > **Note:** The above commands are for Debian/Ubuntu-based distributions. For Fedora, use `sudo dnf install python3`. For Arch Linux, use `sudo pacman -S python`.

3. Verify the installation by running `python3 --version` on the terminal.
   The output should be `Python 3.10.0` (or whichever version was installed).

   > **Note:** On Linux, Python is typically invoked as `python3` rather than `python`.

#### MacOS

1. Open a terminal and run the following command to check if Python is already installed:
   `python3 --version`.
   If Python 3.10 or higher is already installed, you can skip the steps below.

2. It is recommended to install Python via [**Homebrew**](https://brew.sh/). If you don't have Homebrew installed, run:

    ```bash
    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
    ```

   Then install Python with:

    ```bash
    brew install python
    ```

   Alternatively, you can download the macOS installer directly from [**python.org**](https://www.python.org/downloads/) and follow the installation wizard.

3. Verify the installation by running `python3 --version` on the terminal.
   The output should be `Python 3.10.0` (or whichever version was installed).

   > **Note:** On macOS, `python` may point to the system Python 2 installation. Always use `python3` to ensure you are using the correct version.

### Python environment

TL;DR:

```bash
python -m venv venv
venv\Scripts\activate
pip install numpy
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

    > **Note:** You can use AI agents to help you write the code, but remember that any AI usage must be reported explicitly in the report.

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
