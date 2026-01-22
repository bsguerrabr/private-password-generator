# Private Password Generator

A privacy-focused password generator. Passwords are generated locally in your browser using the Web Crypto API and are never stored or sent to any server.

## Features

- **100% Client-Side**: Passwords are generated in your browser using JavaScript
- **Cryptographically Secure**: Uses `crypto.getRandomValues()` (Web Crypto API)
- **No Tracking**: No analytics, no cookies, no data collection
- **Customizable**: Choose password length (1-50 characters) and character types (letters, numbers, symbols)

## Run Locally

```bash
# Create virtual environment
python -m venv venv

# Activate virtual environment (Windows)
venv\Scripts\activate

# Activate virtual environment (macOS/Linux)
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Run the server
python app.py
```

The site will be available at `http://127.0.0.1:5000`

## Tech Stack

- **Backend**: Flask (Python) - serves the static HTML page
- **Frontend**: Vanilla JavaScript - handles password generation
- **Security**: Web Crypto API for cryptographic randomness
