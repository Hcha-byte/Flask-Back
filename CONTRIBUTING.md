# Contributing to Flask-Back

Thank you for your interest in contributing to **Flask-Back**! This guide outlines how you can help improve the project.

---

## 🧰 Requirements

Before contributing, make sure you have:

* Python 3.8+ installed
* [Poetry](https://python-poetry.org/) or `pip` with virtualenv
* A GitHub account

Clone the repo and install dependencies:

```bash
git clone https://github.com/Hcha-byte/Flask-Back.git
cd Flask-Back
python -m venv .venv
source .venv/bin/activate
pip install -e ".[dev]"
```

---

## 📦 Running Tests

Run all tests:

```bash
pytest
```

Check code coverage:

```bash
pytest --cov=src --cov-report=term-missing
```

---

## 🔧 Making Changes

* Fork the repository and create your branch from `main`.
* Make sure your changes are tested.
* Follow PEP8 conventions.

---

## 📄 Docs

If you update or add features, please update the documentation or open an issue requesting help with it.

---

## ✅ Submitting a Pull Request

1. Push your branch to GitHub
2. Open a Pull Request with a clear title and description
3. Reference related issues when applicable

---

## 💬 Questions & Feedback

Open an issue or discussion at:
[https://github.com/Hcha-byte/Flask-Back/issues](https://github.com/Hcha-byte/Flask-Back/issues)

---

Thanks for helping improve Flask-Back! 🙌
