cd /home/student/mission3/tier3
cat << 'EOF' > tier3_environment_explorer.md
# Tier 3 — Applied Project: Environment Explorer

## 1. Python Development Environments
A code editor or Integrated Development Environment (IDE) gives you a workspace to write, save, organize, and run Python programs.

* **IDLE (Integrated Development and Learning Environment):** Included automatically when Python is installed. Great for beginners testing single lines in the interactive shell (`>>>`) and writing or running small scripts without extra setup.
* **Visual Studio Code (VS Code):** A free, lightweight code editor by Microsoft. When paired with the official Python extension, it supports code completion, integrated terminals, and project workflows.
* **PyCharm (Community Edition):** A dedicated Python IDE by JetBrains. Useful for larger Python projects, visual debugging, code inspection, and structured project/environment management.



## Creating and Running a Script (`hello.py`)

### In IDLE
1. Open **IDLE** and click **File > New File** to open a blank script window.
2. Type `print("Hello, Python!")` into the script window.
3. Save the file as `hello.py` (**File > Save**) and press **F5** (or select **Run > Run Module**) to display `Hello, Python!` in the IDLE shell.

### In Terminal / VS Code (Step-by-Step)
Copy and paste these commands into your terminal to create a project folder, write `hello.py`, and execute it:

```bash
mkdir -p python_launchpad_demo
cd python_launchpad_demo
cat << 'PYEOF' > hello.py
print("Hello, Python!")
PYEOF
python3 hello.py
```

### What Each Step Does

mkdir -p python_launchpad_demo: Creates a folder named python_launchpad_demo to keep your project files together (and avoids an error if the folder already exists).

cd python_launchpad_demo: Moves your terminal into python_launchpad_demo so commands run inside that folder.

cat << 'PYEOF' > hello.py ... PYEOF: Writes print("Hello, Python!") into a new file named hello.py.

python3 hello.py: Runs hello.py using the Python 3 interpreter so Hello, Python! prints on screen


### Creating and Using a Virtual Environment (venv)

Why Virtual Environments Matter

Different projects can require different versions of the same package. A virtual environment (venv) creates an isolated folder inside a project with its own Python setup and installed packages so one project's dependencies do not interfere with another project or your system Python.
Step 1: Create the Virtual Environment (macOS / Linux / Git Bash)

Copy and paste these commands into your terminal:

```Bash
cd python_launchpad_demo
python3 -m venv .venv
ls -la .venv
```
### What Each Step Does:

cd python_launchpad_demo: Moves into your project directory so the virtual environment is created inside the project rather than scattered across your computer.

python3 -m venv .venv: Uses Python's built-in venv module (-m venv) to create a new virtual environment directory named .venv.

ls -la .venv: Lists the files and subfolders inside .venv (such as bin, include, and pyvenv.cfg) What Each Step Does:

cd python_launchpad_demo: Moves into your project directory so the virtual environment is created inside the project rather than scattered across your computer.

python3 -m venv .venv: Uses Python's built-in venv module (-m venv) to create a new virtual environment directory named .venv.

ls -la .venv: Lists the files and subfolders inside .venv (such as bin, include, and pyvenv.cfg) so you can confirm the environment was created.

so you can confirm the environment was created.


### Activate and Work Inside the Environment (macOS / Linux / Git Bash)
```Bash
source .venv/bin/activate
which python
python3 -m pip install --upgrade pip
pip install requests
pip list
deactivate
```
###  What Each Step Does:

source .venv/bin/activate: Activates the .venv virtual environment in the current shell session so python and pip point to .venv.

which python: Shows the path of the active python executable so you can verify it is coming from inside .venv.

python3 -m pip install --upgrade pip: Upgrades pip inside the virtual environment using the active Python interpreter.

pip install requests: Installs the requests package inside .venv only.

pip list: Prints the packages installed inside the active environment.

deactivate: Exits .venv and returns your terminal to its normal system state.



### Windows (Command Prompt) Equivalent

On Windows Command Prompt, the creation, activation, and package commands look like this:
DOS
```Bash
cd python_launchpad_demo
python -m venv .venv
.venv\Scripts\activate
python -m pip install --upgrade pip
pip install requests
pip list
deactivate
```

### What Each Step Does on Windows:

cd python_launchpad_demo: Moves into your project folder.

python -m venv .venv: Creates the .venv virtual environment using Windows' python command.

.venv\Scripts\activate: Runs Windows' activation script inside .venv\Scripts to turn on the virtual environment.

python -m pip install --upgrade pip: Updates pip inside the active environment.

pip install requests: Installs requests inside .venv.

pip list: Shows installed packages in .venv.

deactivate: Leaves the virtual environment.