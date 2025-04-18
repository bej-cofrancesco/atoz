# Python Installation Guide

## Required Software

- **Python**: Download and install from [python.org](https://www.python.org/downloads/) (version 3.9+ recommended)
- **pip**: Package manager (included with Python installation)
- **Virtual Environment**: `python -m venv` (included with Python)

## File Extensions

- `.py` - Python source files
- `.ipynb` - Jupyter notebook files
- `.pyc` - Compiled Python files (generated automatically)
- `.pyd` - Python dynamic module (Windows)
- `.pyx` - Cython source files

## Package Management

```bash
# Create a virtual environment
python -m venv venv

# Activate virtual environment
# Windows
venv\Scripts\activate
# macOS/Linux
source venv/bin/activate

# Install packages
pip install package-name

# Save dependencies
pip freeze > requirements.txt

# Install from requirements
pip install -r requirements.txt
```

## Running Python Programs

```bash
# Run a script
python script.py

# Run the interactive interpreter
python

# Run a module
python -m module_name
```

## Common Libraries

- **Web Development**: Django, Flask, FastAPI
- **Data Science**: NumPy, Pandas, Matplotlib
- **Machine Learning**: TensorFlow, PyTorch, scikit-learn
- **Testing**: pytest, unittest
