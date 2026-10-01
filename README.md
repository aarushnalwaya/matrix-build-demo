# Matrix Builds for Multi-Environment Testing

## Objective

The objective of this assignment is to implement a GitHub Actions matrix build that executes the same Python unit test suite across multiple operating systems and Python versions simultaneously.

## Project Description

This project contains a simple Python calculator with three mathematical operations:

- Addition
- Subtraction
- Multiplication

Unit tests are written using `pytest`.

GitHub Actions is configured with a matrix strategy to test the project across:

- Ubuntu
- Windows

and the following Python versions:

- Python 3.10
- Python 3.11
- Python 3.12

This results in:

**2 operating systems × 3 Python versions = 6 test environments**

Matrix Test Results
Screenshot 1 — Six Matrix Jobs Completed Successfully

<img width="1904" height="848" alt="Screenshot 2026-10-01 134622" src="https://github.com/user-attachments/assets/f17c20b6-3d0a-41b0-9057-e1c8f3c12850" />

Suggested screenshot: GitHub Actions workflow run showing all six jobs with green check marks and the message 6 jobs completed.

Screenshot 2 — Matrix Configuration

<img width="1373" height="919" alt="Screenshot 2026-10-01 134729" src="https://github.com/user-attachments/assets/e2d4f683-0873-4e86-8cbd-c91d8ed3fc87" />

Suggested screenshot: GitHub Actions Workflow file page showing the strategy.matrix configuration and the six generated jobs in the left panel.

## Project Structure

```text
matrix-build-demo/
│
├── .github/
│   └── workflows/
│       └── test.yml
│
├── calculator.py
├── test_calculator.py
└── README.md
