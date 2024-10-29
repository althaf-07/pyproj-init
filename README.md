# pyproj-init

`pyproj-init` is a Python script for quickly setting up the directory structure, virtual environment, and Git repository for a new Python project.

## Features

- Creates a consistent folder structure with directories like `src`, `config`, and `tests`.
- Generates essential files such as `.gitignore`, `requirements.txt`, `LICENSE`, `pyproject.toml`, and `README.md`.
- Sets up a Python virtual environment in `.venv` and initializes a Git repository.
- Automatically updates `.gitignore` to include `.venv`.

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/althaf-07/pyproj-init.git
    ```

2. Move the script to `/usr/local/bin` for easy access:

    ```bash
    mv pyproj-init/pyproj-init /usr/local/bin/
    ```

## Usage

Run `pyproj-init` from the command line, specifying the path where you want to create the project structure.

### Options for Using `pyproj-init`

1. **Specify a Full Path for the Project Folder**

    Use this command to set up the project structure at a specified full path. The script will create the directory if it doesn’t exist:

    ```bash
    pyproj-init /path/to/your_project
    ```

2. **Create the Project Folder in the Current Directory**

    Create a project folder with a specified name in your current directory:

    ```bash
    pyproj-init your_project
    ```

3. **Initialize the Current Directory as a Project Folder**

    If you're already inside the directory you want to initialize, simply use:

    ```bash
    pyproj-init .
    ```

## Project Structure

Running `pyproj-init` generates the following structure:

```
your_project/
├── .gitignore
├── LICENSE
├── README.md
├── pyproject.toml
├── requirements.txt
├── src/
│   ├── __init__.py
│   └── main.py
├── config/
├── tests/
│   ├── __init__.py
│   └── test_main.py
└── .venv/
```

## Example Output

Upon running `pyproj-init`, you’ll see output similar to:

```plaintext
Created directory: /path/to/your_project/src
Created directory: /path/to/your_project/config
Created directory: /path/to/your_project/tests
Created file: /path/to/your_project/.gitignore
Created file: /path/to/your_project/requirements.txt
Created file: /path/to/your_project/LICENSE
Created file: /path/to/your_project/pyproject.toml
Created file: /path/to/your_project/README.md
Created file: /path/to/your_project/src/__init__.py
Created file: /path/to/your_project/src/main.py
Created file: /path/to/your_project/tests/__init__.py
Created file: /path/to/your_project/tests/test_main.py
Created virtual environment: /path/to/your_project/.venv
Initialized git repository in: /path/to/your_project
Updated .gitignore to include .venv
Project 'your_project' structure setup completed successfully!
```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

