# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Important Rules

- **Python packages must only be installed inside a virtual environment.** Never run `pip install` without first activating a venv.
- **All code and text must be in English.** This project targets a global audience.

## Project Overview

Password generator website using Flask. The password is generated on the client side (JavaScript) for maximum privacy - it never passes through the server.

## Build & Run Commands

```bash
# Create virtual environment (first time only)
python -m venv venv

# Activate virtual environment (Windows)
venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the server
python app.py
```

The site will be available at `http://127.0.0.1:5000`

## Architecture

- **app.py**: Flask server that only serves the HTML page
- **templates/index.html**: Single page containing all the interface and password generation logic in JavaScript
- Generation uses `crypto.getRandomValues()` (Web Crypto API) for cryptographic security
