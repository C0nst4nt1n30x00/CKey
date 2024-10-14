# API Caller Tool

## Overview

The **LeakMe** is a Python script designed to interact with various APIs by simplifying the process of making requests. The tool provides a user-friendly command-line interface that allows users to select from a list of supported APIs, input their credentials, and execute API calls easily.

## Supported APIs

This tool currently supports the following APIs:

1. **Bing**
2. **Cloudflare**
3. **Datadog**
4. **Facebook Access Token**
5. **Facebook App Secret**
6. **GitHub Client ID and Secret**
7. **GitLab**
8. **HubSpot API Key**
9. **Stripe**
10. **Twitter API Secret**

## Features

- **Interactive CLI**: Choose from a list of APIs to make requests.
- **Dynamic URL Generation**: The script constructs API endpoints based on user input.
- **Simple Authentication**: Provides a straightforward way to input API keys and tokens.

## Requirements

- Python 3.x
- `curl` installed on your system

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/psuedoF/leakme
   cd leakme
   chmod +x leakme.py
