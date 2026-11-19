Personal Finance Tracker (MIT103 Assessment 3, Phase 2)
A console Personal Finance Tracker for Google Colab. It records income and expenses, saves them to CSV, and limits what each user can do by role.
Features
- Admin: add, display, search and delete transactions. Viewer: display and search only.
- CSV storage using csv.DictReader and csv.DictWriter.
- Salted PBKDF2 password verification (hashlib.pbkdf2_hmac, hmac.compare_digest).
- Input validation and clear messages for malformed CSV rows.
- Category totals using a dictionary.
How to run (Google Colab)
1. Open the notebook in Google Colab.
2. Upload MIT103_A3_Revised_T3_2026_Sample_Transactions.csv to the Files panel.
3. Run all cells. On the first run you choose passwords for the demo accounts admin and viewer. Only salted hashes are stored.
4. Log in and use the menu.
Data and restoring it
The sample CSV is read-only. Changes are saved to my_transactions.csv in Google Drive (MyDrive/FinanceTracker). On a fresh Colab runtime, mount Drive and run again, or re-upload the saved working CSV.
Safety
All data is fictional. No passwords are stored in the code or in this repository. demo_accounts.json is excluded by .gitignore.
