# TIER 5 — ARCHITECTURE/SYSTEM CHALLENGE
# PYTHON LAUNCHPAD TEAM PROJECT

## 1. Introduction to Python

Python is a high-level, general-purpose programming language known for its simple and readable syntax.

It was created by Guido van Rossum and first released in 1991.

Python is popular because beginners can learn it easily, while experienced developers can use it to build complex applications.

### Importance of Python

Python is used in different areas of technology, including:

- Artificial Intelligence (AI)
- Machine Learning (ML)
- Web development
- Data analysis
- Automation
- Software development
- Scientific computing

Python is also supported by a large community and provides many libraries and tools that make programming easier.

---

## 2. Installing Python on Different Operating Systems

Python can be installed on Windows, macOS, and Linux.

### A. Installing Python on Windows

1. Open a web browser.
2. Visit https://www.python.org/downloads/
3. Download the latest stable Python release for Windows.
4. Open the downloaded installer.
5. Select the option to add Python to PATH.
6. Click Install Now.
7. Wait for the installation to finish.
8. Open Command Prompt.
9. Type:

   `python --version`

If a Python version appears, the installation was successful.

### B. Installing Python on macOS

1. Visit https://www.python.org/downloads/macos/
2. Download the appropriate Python installer.
3. Open the downloaded package.
4. Follow the installation instructions.
5. Open Terminal.
6. Type:

   `python3 --version`

If the version number appears, Python is installed successfully.

### C. Installing Python on Linux

Many Linux distributions include Python 3 or provide it through their package managers.

For Ubuntu and other Debian-based distributions:

1. Open the terminal.
2. Update the package list:

   `sudo apt update`

3. Install Python:

   `sudo apt install python3`

4. Install pip and virtual environment support:

   `sudo apt install python3-pip python3-venv`

5. Check the installation:

   `python3 --version`

If the version number appears, Python is ready to use.

---

## 3. Using IDLE

IDLE stands for Integrated Development and Learning Environment.

It is a basic development environment that comes with many standard Python installations.

### What is IDLE used for?

IDLE allows beginners to:

- Write Python code.
- Run Python programs.
- Test small pieces of code.
- Identify syntax errors.
- Learn Python interactively.

### How to create and run a script in IDLE

1. Open IDLE from your computer's applications.
2. Select File.
3. Click New File.
4. Type the following code:

   `print("Hello, Python!")`

5. Save the file as `hello.py`.
6. Select Run.
7. Click Run Module.
8. The output will appear in the Python Shell.

Expected output:

`Hello, Python!`

---

## 4. Other Python IDEs and Text Editors

Apart from IDLE, developers can use other environments to write Python programs.

### A. Visual Studio Code (VS Code)

Visual Studio Code is a lightweight and popular code editor developed by Microsoft.

It supports Python through extensions.

**What it is used for:**

- Writing Python programs.
- Debugging code.
- Managing project files.
- Using Git and GitHub.
- Working with different programming languages.

**How to run a Python script:**

1. Download VS Code from https://code.visualstudio.com/
2. Install Python on your computer.
3. Open VS Code.
4. Install the Python extension.
5. Create a new file called `hello.py`.
6. Type:

   `print("Hello, Python!")`

7. Save the file.
8. Open the terminal in VS Code.
9. Run:

   `python3 hello.py`

Expected output:

`Hello, Python!`

### B. PyCharm

PyCharm is an Integrated Development Environment (IDE) developed by JetBrains.

It provides tools specifically designed for Python development.

**What it is used for:**

- Writing Python applications.
- Debugging programs.
- Managing Python projects.
- Working with virtual environments.
- Testing and organising code.

**How to run a Python script:**

1. Download PyCharm from https://www.jetbrains.com/pycharm/
2. Install and open PyCharm.
3. Create a new Python project.
4. Create a Python file named `hello.py`.
5. Enter:

   `print("Hello, Python!")`

6. Save the file.
7. Right-click the file.
8. Select Run.

Expected output:

`Hello, Python!`

---

## 5. Understanding Virtual Environments

A virtual environment is an isolated Python environment created for a particular project.

It allows a developer to install packages without affecting other Python projects on the computer.

### Why are virtual environments important?

- They prevent package conflicts.
- They keep project dependencies organised.
- They allow different projects to use different package versions.
- They make projects easier to manage.

### Creating a virtual environment

1. Open your project directory in the terminal.
2. Create a virtual environment:

   `python3 -m venv venv`

3. Activate it on Linux or macOS:

   `source venv/bin/activate`

4. On Windows Command Prompt:

   `venv\Scripts\activate.bat`

5. On Windows PowerShell:

   `.\venv\Scripts\Activate.ps1`

When activated, the environment name usually appears in the terminal prompt.

To deactivate it, type:

`deactivate`

---

## 6. Installing Python Packages

A Python package is a collection of reusable code that provides additional functionality.

Python uses pip, its standard package installer, to install many third-party packages.

### Installing a package

For example, to install the requests package, use:

`python3 -m pip install requests`

### Checking installed packages

Use:

`python3 -m pip list`

### Updating pip

Use:

`python3 -m pip install --upgrade pip`

### Why do we install packages?

Packages help developers avoid writing everything from scratch.

They provide ready-made tools for tasks such as:

- Data analysis
- Web development
- Artificial Intelligence
- Machine Learning
- Automation

When working with a virtual environment, activate it before installing packages so they are installed in the correct project environment.

---

## 7. Creating and Running a Basic Python Script

A Python script is a file containing Python instructions.

Python files normally use the `.py` extension.

### Step 1: Create a file

Create a file named:

`hello.py`

### Step 2: Write the code

Enter:

```python
print("Hello, Python!")
```

### Step 3: Save the file

Save it as `hello.py`.

### Step 4: Open the terminal

Navigate to the directory containing the file.

### Step 5: Run the script

On Linux and macOS:

`python3 hello.py`

On Windows:

`python hello.py`

### Expected output

```text
Hello, Python!
```

The `print()` function displays information on the screen.

---

## 8. Understanding Python Interpreter Architecture

A Python interpreter is a program that processes and executes Python code.

It allows the computer to carry out instructions written in Python.

In the standard CPython implementation, Python code passes through several stages.

### How Python code is executed

1. **Source Code:** The programmer writes instructions in a Python file.
2. **Compilation:** CPython compiles the source code into bytecode.
3. **Bytecode:** Bytecode is an intermediate representation of the program.
4. **Python Virtual Machine:** The Python Virtual Machine executes the bytecode.
5. **Output:** The program produces its result.

### Simple architecture diagram

```text
Python Source Code
        |
        v
   Compilation
        |
        v
     Bytecode
        |
        v
Python Virtual Machine
        |
        v
      Output
```

This process helps Python execute instructions written by developers.

---

## 9. High-Level vs. Low-Level Programming Languages

Programming languages can be grouped according to how close they are to human language or computer hardware.

### High-Level Languages

High-level languages are designed to be easier for humans to read, write, and understand.

Examples include:

- Python
- Java
- JavaScript
- C#

**Characteristics:**

- Readable syntax.
- Easier to learn.
- Generally more abstracted from computer hardware.
- Often require an interpreter or compiler.

### Low-Level Languages

Low-level languages are closer to the instructions understood by computer hardware.

Examples include:

- Machine language
- Assembly language

**Characteristics:**

- Closer to hardware.
- Can provide greater control over system resources.
- Often require more technical knowledge.
- Can be more difficult for beginners to understand.

### Comparison

| High-Level Languages | Low-Level Languages |
|---|---|
| Easier to read | More difficult to read |
| More abstracted from hardware | Closer to hardware |
| Faster to develop with | Often require more detailed instructions |
| Example: Python | Example: Assembly |

---

## 10. Understanding CPython and Bytecode

### What is CPython?

CPython is the standard and most widely used implementation of Python.

It is written mainly in the C programming language.

It translates Python source code into bytecode and executes that bytecode using its virtual machine.

### What is Bytecode?

Bytecode is an intermediate form of instructions generated when Python source code is compiled.

It is not the same as machine code.

The Python Virtual Machine executes the bytecode.

### Why is bytecode important?

- It helps organise Python code for execution.
- It separates source code from the execution process.
- It supports Python's execution model.
- It can be stored in compiled `.pyc` files.

---

## 11. Implementation Speed vs. Execution Speed

These two concepts describe different aspects of programming performance.

### Implementation Speed

Implementation speed refers to how quickly a developer can write, develop, and complete a program.

Python is popular for implementation speed because:

- Its syntax is readable.
- It requires fewer lines of code for many tasks.
- It has many reusable libraries.
- It supports rapid development.

### Execution Speed

Execution speed refers to how quickly a program runs and completes its operations.

Python can be slower than some compiled languages because of its execution model and runtime overhead.

Languages such as C and C++ can offer faster execution for certain tasks.

### Comparison

| Implementation Speed | Execution Speed |
|---|---|
| How quickly code is developed | How quickly code runs |
| Focuses on developer productivity | Focuses on program performance |
| Python is often very productive | Compiled languages may be faster for some workloads |

Both concepts are important when choosing a programming language for a project.

---

## 12. Common Troubleshooting FAQs

### FAQ 1: Why is Python not recognised?

**Possible cause:** Python may not be installed correctly or may not be available through the system PATH.

**Solution:**

- Check whether Python is installed.
- On Windows, check the PATH configuration.
- On Linux and macOS, try `python3 --version`.

### FAQ 2: Why does my Python script not run?

**Possible cause:** The file may contain errors or the terminal may be in the wrong directory.

**Solution:**

- Check the filename.
- Confirm that the file exists.
- Read the error message.
- Check the code for syntax errors.

### FAQ 3: Why does pip fail to install a package?

**Possible cause:** There may be an internet connection problem, an incorrect package name, or an environment issue.

**Solution:**

- Check the internet connection.
- Confirm the package name.
- Update pip.
- Activate the correct virtual environment.

### FAQ 4: Why am I getting a ModuleNotFoundError?

**Possible cause:** The required module may not be installed in the Python environment being used.

**Solution:**

- Identify the missing module.
- Activate the correct environment.
- Install the module using pip.
- Run the program again.

### FAQ 5: Why can I not activate my virtual environment?

**Possible cause:** The activation command may be incorrect for the operating system.

**Solution:**

- Confirm that the virtual environment exists.
- Use the correct activation command.
- On Windows PowerShell, check whether script execution restrictions are preventing activation.

---

## 13. Resources and References

The following official resources were used as references for this guide:

1. Python Official Website: https://www.python.org/
2. Python Downloads: https://www.python.org/downloads/
3. Python Documentation: https://docs.python.org/3/
4. Python Tutorial: https://docs.python.org/3/tutorial/
5. Python Virtual Environments: https://docs.python.org/3/library/venv.html
6. Visual Studio Code: https://code.visualstudio.com/
7. PyCharm: https://www.jetbrains.com/pycharm/

These resources provide additional information about Python installation, development environments, programming concepts, and troubleshooting.

---

## 14. Squad Roles and Responsibilities

The project requires a squad of 2–5 members.

The following responsibilities should be assigned among the actual team members.

| Role | Responsibility | Assigned Member |
|---|---|---|
| Project Manager | Coordinates the project and ensures deadlines are met. | To be assigned |
| Technical Writer | Prepares and organises the beginner's guide. | To be assigned |
| Video Producer | Records and edits the demonstration video. | To be assigned |
| Research Specialist | Checks technical information and references. | To be assigned |
| Quality Assurance | Reviews the guide, script, and video for errors. | To be assigned |

When the squad has fewer than five members, responsibilities can be combined.

---

## 15. Video Demonstration Plan

### Video Title: Getting Started with Python — Python Launchpad

**Target duration:** 5–10 minutes.

### Part 1: Introduction (0:00–0:45)

Introduce the project and explain what Python is.

Briefly describe why Python is useful for beginners and developers.

### Part 2: Python Installation (0:45–2:30)

Demonstrate the installation process on the chosen operating system.

Explain where Python can be downloaded and how to confirm that installation was successful.

### Part 3: Introducing the Development Environment (2:30–4:00)

Introduce the chosen editor, such as Visual Studio Code or IDLE.

Explain the main features used to write and run Python programs.

### Part 4: Creating a Python Script (4:00–5:30)

Create a file named `hello.py`.

Enter:

```python
print("Hello, Python!")
```

Explain what the `print()` function does.

### Part 5: Running the Script (5:30–7:00)

Open the terminal and run the script.

For Linux and macOS:

`python3 hello.py`

For Windows:

`python hello.py`

Show the output:

```text
Hello, Python!
```

Explain that Python processes the instructions and displays the result.

### Part 6: Conclusion (7:00–8:00)

Summarise what was demonstrated:

- Python installation.
- Development environment.
- Creating a Python script.
- Running a Python program.
- Understanding the output.

Thank viewers for watching.

---

## 16. Final Quality Assurance Checklist

Before submitting the project, confirm the following:

- [ ] The guide introduces Python and its importance.
- [ ] Installation instructions cover Windows, macOS, and Linux.
- [ ] IDLE is explained.
- [ ] At least two alternative development environments are included.
- [ ] Virtual environments are explained.
- [ ] Package installation is demonstrated.
- [ ] A basic Python script is included.
- [ ] Interpreter architecture is explained.
- [ ] High-level and low-level languages are compared.
- [ ] CPython and bytecode are explained.
- [ ] Implementation speed and execution speed are discussed.
- [ ] Troubleshooting FAQs are included.
- [ ] Resources and references are documented.
- [ ] Squad responsibilities are assigned.
- [ ] The demonstration video is between 5 and 10 minutes.
- [ ] The video has clear visuals and audio.
- [ ] The Python script runs successfully.
- [ ] All files are accessible to reviewers.
- [ ] The final submission is uploaded to the classroom.

---

## 17. Conclusion

The Python Launchpad Team Project brings together important concepts that beginners need when starting their Python programming journey.

It explains how to install Python, choose a development environment, create and execute scripts, manage virtual environments, and install packages.

It also introduces the internal workings of Python, including CPython, bytecode, and interpreter architecture.

Through the written guide and video demonstration, beginners can develop practical skills and gain confidence working with Python.

**Python Launchpad: Start Learning. Start Building. Start Creating.**