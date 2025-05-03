# hotmail-checker
A fast and efficient Python tool for validating Hotmail/Outlook email accounts by attempting SMTP login. This project checks email:password combinations, identifies valid and invalid accounts, and saves results to separate output files. Built with multithreading for high performance, it’s designed for security researchers, account managers, or educational purposes.

# Features
Bulk Email Checking: Validates multiple Hotmail/Outlook accounts from a text file.
SMTP Authentication: Uses smtplib to verify login credentials via smtp-mail.outlook.com.
Multithreaded Processing: Leverages concurrent.futures.ThreadPoolExecutor with up to 100 workers for rapid checks.
Colorful CLI Output: Displays results in a user-friendly format using colorama.
Result Logging: Saves valid accounts to live.txt and invalid ones to dead.txt.
