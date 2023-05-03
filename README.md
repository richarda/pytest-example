## Pytest example

This is a simple calculator module to show how [coverage.py](https://coverage.readthedocs.io/en/latest/) and [pytest](https://docs.pytest.org/en/latest/) can be used.

## Getting Started

To run the unit tests and generate a coverage report, follow these steps:

1. Clone the repository:


2. Create a virtual environment and activate it:
```
python3 -m venv venv
source venv/bin/activate # On Windows, use venv\Scripts\activate
```

3. Install the required dependencies:

```
pip install -r requirements.txt
```

4. Run the unit tests with coverage:

```
coverage run -m pytest
```

5. Generate a coverage report:

```
coverage report
```


This will run the unit tests and display the coverage report in your terminal.

```zsh
(venv) ➜ /workspaces/pytest-example (main) $ coverage run -m pytest
================ test session starts ====================================================
platform linux -- Python 3.10.4, pytest-7.3.1, pluggy-1.0.0
rootdir: /workspaces/pytest-example
plugins: cov-4.0.0
collected 4 items                                                                                                                       

test_calculator.py .... [100%]

================= 4 passed in 0.02s ==================
(venv) ➜ /workspaces/pytest-example (main) $ coverage report
Name                 Stmts   Miss  Cover
----------------------------------------
calculator.py            2      0   100%
test_calculator.py      10      0   100%
----------------------------------------
TOTAL                   12      0   100%
```

