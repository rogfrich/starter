# Starter
A simple utility to scaffold new Python projects. 

# Usage
`python3 starter.py [-gh] <projectname>`

This will create a new folder called <projectname> in the configured directory, with a useful set of standard files such as `README.md`, requirements files etc.

Options:
-  `-g` initialise a git repo in the new directory.
- `-h` display help

# Configuration
Configuration is via the environment variables set in `.env` which is a file in the same directory as the main `starter.py` module:
- `STANDARD_CODE_DIR` is the folder in which the new project directory will be created.
- `TEMPLATE_DIRECTORY` is where Starter looks for template files for:
  - `.gitignore`
  - `requirements.txt`
  - `requirements-dev.txt`

The template files can be blank, but they must exist in the specified `TEMPLATE_DIRECTORY`.

## Example configuration
```
STANDARD_CODE_DIR=/Path/to/where/you/keep/your/code
TEMPLATE_DIRECTORY=/Path/to/where/you/keep/your/templates
```
Best practice would be to not commit `.env` to GitHub.


