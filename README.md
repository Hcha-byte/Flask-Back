# Flask-Back

A lightweight Flask extension for managing back URLs between pages.

## Features
- Saves "back" URLs automatically or manually
- Template injection: `{{ back_url }}`
- Optional referrer fallback
- Easy to exclude endpoints from tracking

## Installation

```bash
pip install flask-back
```

## Example

```python
from flask import Flask, redirect
from flask_back import Back

app = Flask(__name__)
app.secret_key = "..."

back = Back(app, default_url="/", use_referrer=True)

@app.route("/save")
@back.save_url
def save_page():
    return "Saved this as a back URL."

@app.route("/go-back")
def go_back():
    return redirect(back.get_url())

@app.route("/excluded")
@back.exclude
def excluded_page():
    return "This page won't be saved as back URL."
```