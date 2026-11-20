# Tier 4 — Problem-Solving Challenge: Python Troubleshooting Desk

## Introduction

Python is a popular programming language, but beginners may sometimes experience difficulties when installing, setting up, or running it.

This troubleshooting guide explains common Python problems, their possible causes, and simple steps learners can follow to resolve them.

The goal is to help beginners understand how to identify problems and solve them independently.

---

## 1. Problem: Python Is Not Installed

**Description:**

A learner tries to run Python but receives an error because Python is not installed on their computer.

**Possible Cause:**

Python has not been downloaded or installed.

**Solution:**

1. Visit the official Python website: https://www.python.org/downloads/
2. Download the appropriate Python version for your operating system.
3. Run the installer.
4. Follow the installation instructions.
5. Open the terminal.
6. Type `python --version` or `python3 --version` to check whether Python is installed.

If the version number appears, Python has been installed successfully.

---

## 2. Problem: Python Command Is Not Recognised

**Description:**

A learner types `python` in the terminal but receives a message saying that the command is not recognised or not found.

**Possible Cause:**

Python may not have been added to the system PATH, or the learner may be using the wrong command.

**Solution:**

1. Check whether Python is installed.
2. On Windows, ensure that Python was added to PATH during installation.
3. On Linux or macOS, try using `python3` instead of `python`.
4. Restart the terminal after making changes.
5. Run `python --version` or `python3 --version` again.

---

## 3. Problem: Virtual Environment Cannot Be Activated

**Description:**

A learner creates a virtual environment but cannot activate it.

**Possible Cause:**

The activation command may be incorrect for the operating system, or the virtual environment may not have been created successfully.

**Solution:**

1. Open the project directory in the terminal.
2. Create a virtual environment using:

   `python3 -m venv venv`

3. On Linux or macOS, activate it using:

   `source venv/bin/activate`

4. On Windows Command Prompt, use:

   `venv\Scripts\activate.bat`

5. On Windows PowerShell, use:

   `.\venv\Scripts\Activate.ps1`

6. Check that the environment is active. Its name should usually appear at the beginning of the terminal prompt.

---

## 4. Problem: Package Installation Fails

**Description:**

A learner tries to install a Python package using pip but receives an error.

**Possible Cause:**

- There may be no internet connection.
- pip may be outdated.
- The package name may be incorrect.
- The learner may be using the wrong Python environment.

**Solution:**

1. Check your internet connection.
2. Confirm that the package name is correct.
3. Update pip using:

   `python3 -m pip install --upgrade pip`

4. Install the required package using:

   `python3 -m pip install package_name`

5. If using a virtual environment, activate it before installing the package.

---

## 5. Problem: Python Cannot Find a Script

**Description:**

A learner tries to run a Python file but receives an error saying that the file cannot be found.

**Possible Cause:**

The learner may be in the wrong directory or may have typed the filename incorrectly.

**Solution:**

1. Check the current directory using:

   `pwd`

2. List the files in the directory using:

   `ls`

3. Confirm that the Python file exists.
4. Move into the correct directory using `cd directory_name`.
5. Run the script using:

   `python3 filename.py`

Make sure the filename and its extension are correct.

---

## 6. Problem: Python Script Produces an Error

**Description:**

A learner runs a Python script, but the program stops and displays an error message.

**Possible Cause:**

The code may contain a syntax error, incorrect variable name, indentation problem, or invalid operation.

**Solution:**

1. Read the error message carefully.
2. Check the line number mentioned in the error.
3. Look for spelling mistakes and missing brackets or quotation marks.
4. Check that indentation is correct.
5. Confirm that variables are written consistently.
6. Correct the problem and run the script again.

For example:

Incorrect code:

`print("Hello, Python!"`

Correct code:

`print("Hello, Python!")`

The incorrect example is missing a closing parenthesis.

---

## 7. Problem: Module Not Found Error

**Description:**

A learner runs a Python script and receives a `ModuleNotFoundError` message.

**Possible Cause:**

The required module may not be installed, or it may have been installed in a different Python environment.

**Solution:**

1. Identify the missing module from the error message.
2. Activate the correct virtual environment if one is being used.
3. Install the missing module using:

   `python3 -m pip install module_name`

4. Run the script again.
5. If the error continues, confirm that the package is installed in the same environment being used to run the script.

---

## 8. Best Practices for Avoiding Python Problems

Beginners can reduce common Python problems by following these practices:

- Download Python from its official website.
- Check the Python version after installation.
- Use virtual environments to organise project dependencies.
- Install packages using pip.
- Keep Python and pip updated.
- Check filenames and directory locations before running scripts.
- Read error messages instead of ignoring them.
- Save files regularly.
- Test programs after making changes.

---

## Conclusion

Troubleshooting is an important part of learning Python. Beginners may experience installation errors, environment problems, package installation failures, or errors when running scripts.

Understanding the possible causes of these problems makes it easier to find solutions.

With regular practice, patience, and proper problem-solving skills, learners can become more confident working with Python independently.

**The key lesson is that errors are part of programming. Instead of giving up, learn to understand the error, identify its cause, and work towards a solution.**