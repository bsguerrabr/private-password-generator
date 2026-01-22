# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Important Rules

- **All code and text must be in English.** This project targets a global audience.

## Project Overview

Privacy-focused password generator. Static site (HTML/CSS/JavaScript only) hosted on Cloudflare Pages. Passwords are generated client-side using the Web Crypto API - nothing is sent to any server.

## Run Locally

Open `index.html` in a browser. No build process or server required.

## Architecture

- **index.html**: Single page containing all HTML, CSS, and JavaScript
- Generation uses `crypto.getRandomValues()` (Web Crypto API) for cryptographic security
