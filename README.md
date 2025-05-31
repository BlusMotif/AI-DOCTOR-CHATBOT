# Medi Chat - Health Chatbot

## Overview
Medi Chat is an AI-powered chatbot designed to assist users with health concerns by providing information based on a comprehensive medical knowledge base.

## Running the Application

To run the application in a production environment, use a WSGI server like Gunicorn or Waitress. Here are example commands to run the application:

### Using Gunicorn (Unix-based systems)
```bash
gunicorn -w 4 app:app
```

### Using Waitress (Windows)
1. Install Waitress:
   ```bash
   pip install waitress
   ```
2. Verify the installation:
   ```bash
   pip show waitress
   ```
3. Run the application:
   ```bash
   waitress-serve --port=5000 app:app
   ```

If you encounter an error stating that `waitress-serve` is not recognized, ensure that your Python Scripts directory is included in your system's PATH environment variable. This directory is typically located at:
```
C:\Users\<YourUsername>\AppData\Local\Programs\Python\Python<version>\Scripts
```
Replace `<YourUsername>` and `<version>` with your actual username and Python version.

### Checking Python Version
To check the version of Python installed on your system, run the following command in your command prompt or terminal:
```bash
python --version
```
or
```bash
python -V
```
If you have multiple versions of Python installed, you might need to specify `python3`:
```bash
python3 --version
```

Adjust the number of workers based on your server's capabilities.
