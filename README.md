# Bankist App

This is a simple banking app simulation built with HTML, CSS, and JavaScript.

## What it does

- **User Login:** Users can log in with a username (derived from their name initials) and a 4-digit PIN.
- **Display Account Movements:** Shows all deposits and withdrawals as a list. Each entry shows if it was a deposit or withdrawal and the amount.
- **Calculate and Display Balance:** Sums all movements to show the current balance.
- **Summary:** Displays total money deposited, total money withdrawn, and interest earned on deposits. Interest is calculated per deposit using a fixed interest rate and only amounts to interest if it is at least 1 unit.
- **Money Transfer:** Logged-in users can transfer money to other users if they have enough balance and the recipient exists.
- **Loan Requests:** Users can request a loan, but the amount must be less than or equal to 10 times the largest deposit made.
- **Account Closure:** Users can close their account by confirming their username and PIN. This deletes their data from the system.
- **Sorting Movements:** The list of transactions can be sorted in ascending order.

## How it works

- Data for each account includes owner name, movements (array of deposits and withdrawals), interest rate, PIN, and account type.
- On login, the app verifies username and PIN, then displays user-specific data.
- Movements are rendered dynamically in the UI, with deposits and withdrawals styled differently.
- Transfers and loans update the movements array and refresh the UI immediately.
- Closing an account removes it from the stored accounts list and hides the interface.
- Sorting toggles the order of transaction display.

## Testing User Accounts

To test the app’s features, use one of the predefined accounts below. Usernames are generated from the owners’ full names by taking the first letter of each name part, all lowercase.

| Owner                 | Username | PIN  | Account Type |
|-----------------------|----------|------|--------------|
| Jonas Schmedtmann     | js       | 1111 | premium      |
| Jessica Davis         | jd       | 2222 | standard     |
| Steven Thomas Williams | stw      | 3333 | premium      |
| Sarah Smith           | ss       | 4444 | basic        |

### 🔗 Live Demo
[Play it here](https://abderrahman-bouhmad.github.io/BANKIST-APP)
