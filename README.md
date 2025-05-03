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


Ensure `emails.txt` is in the project directory with `email:password` combinations.

---

## Usage

1. Prepare `emails.txt` with `email:password` combinations (one per line), e.g.:

    ```
    user1@hotmail.com:password123
    user2@outlook.com:pass456
    ```


2. Check results:
   - Valid accounts are saved to `live.txt`.
   - nvalid accounts are saved to `dead.txt`.
   - Console output shows login success or error messages with color coding.

---

## Example Output

user1@hotmail.com:password123 -> Login Success
user2@outlook.com:pass456 -> Authentication failed.


---

## Disclaimer

This tool is for **educational purposes only**. Unauthorized use for illegal activities, such as unauthorized account access, is strictly prohibited.  
The author is **not responsible** for any misuse. Ensure you have permission to test the accounts you are checking.

---

## Contributing

Contributions are welcome! Feel free to:

- Create pull requests to enhance functionality or fix issues.

---

## Contact

- Telegram: [@azizos](https://t.me/azizos)

---
