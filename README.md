# hotmail-checker
A fast and efficient Python tool for validating Hotmail/Outlook email accounts by attempting SMTP login. This project checks email:password combinations, identifies valid and invalid accounts, and saves results to separate output files. Built with multithreading for high performance, it’s designed for security researchers, account managers, or educational purposes.

## Features

- **Bulk Email Checking**: Validates multiple Hotmail/Outlook accounts from `emails.txt`.
- **SMTP Authentication**: Uses `smtplib` to verify login credentials via `smtp-mail.outlook.com` (port 587).
- **Multithreaded Processing**: Utilizes `concurrent.futures.ThreadPoolExecutor` with up to 100 workers for rapid checks.
- **Colorful CLI Output**: Displays results with `colorama` for clear success/error visualization.
- **Result Logging**: Saves valid accounts to `live.txt` and invalid ones to `dead.txt`.
- **Windows Support**: Includes `run.bat` for easy execution on Windows.

## Repository Contents

- `main.py`: Core script for checking email accounts.
- `requirements.txt`: Lists required Python packages.
- `emails.txt`: Input file for `email:password` combinations.
- `run.bat`: Batch file to run the tool on Windows.
- `Maill-access-Checker.zip`: Archived version of the project.

## Requirements

- Python 3.6+
- Dependencies listed in `requirements.txt`

## Installation

```bash
git clone https://github.com/azizos001/hotmail-checker.git
cd hotmail-checker
pip install -r requirements.txt

