# Jupyter Notebook Test Project

This repository contains a test project for experimenting with [Jupyter Notebooks](https://jupyter.org/), using Python, [pandas](https://pandas.pydata.org/), and [venv](https://docs.python.org/3/library/venv.html) for virtual environment management. Source control is managed with [git](https://git-scm.com/).

## Project Structure

```
.
├── test.ipynb
├── env/                # Python virtual environment (excluded from git)
├── requirements.txt    # Python dependencies
├── .gitignore
└── README.md
```

## Getting Started

### 1. Clone the repository

```sh
git clone <repository-url>
cd <repository-directory>
```

### 2. Create and activate a virtual environment

```sh
python3 -m venv env
source env/bin/activate  # On Windows: env\Scripts\activate
```

### 3. Install dependencies

If a `requirements.txt` file is present, install all dependencies with:

```sh
pip install -r requirements.txt
```

If you need to create or update `requirements.txt` after installing new packages, run:

```sh
pip freeze > requirements.txt
```

Alternatively, to install specific packages:

```sh
pip install pandas jupyter
```

### 4. Start Jupyter Notebook

```sh
jupyter notebook
```

Open `test.ipynb` in your browser to begin working.

## Notes

- The `env/` directory is excluded from version control via [.gitignore](.gitignore).
- Add any additional dependencies to your environment as needed.
- Use `pip freeze > requirements.txt` to save dependencies if you want to share or reproduce the environment.

## Useful Commands

- **Deactivate virtual environment:**  
  ```sh
  deactivate
  ```
- **Update dependencies:**  
  ```sh
  pip install --upgrade pandas jupyter
  ```
- **Update requirements.txt after installing new packages:**  
  ```sh
  pip freeze > requirements.txt
  ```

## License

This project is for testing and educational purposes.