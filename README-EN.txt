WALLET 4.6 — USER GUIDE
================================

A personal finance app that runs directly in your browser.
All data stays on your device (no server, no cloud).


1. FIRST LAUNCH & SECURITY
----------------------------

When you open the app you can choose to enable a 4-digit PIN protection.

• PIN ON → data is encrypted with AES-256-GCM and stored securely.
  WARNING: if you forget the PIN there is no way to recover your data.
• PIN OFF → data is stored in plain text on the device.

Auto-Lock: you can set a timer (1 / 5 / 15 / 30 minutes) after which
the app locks automatically if you stop using it or switch to another tab.

After too many wrong attempts the keypad is locked for 5 minutes.


2. THE 4 MAIN SCREENS
-----------------------

Navigate by swiping horizontally or tapping the bottom icons:

A) 💸 ACCOUNTS (Cash)
   - View total balance and the list of accounts.
   - Record income, expenses, recurring bills and scheduled payments.
   - Search through recent transactions.

B) 🏦 PROJECTS (Savings)
   - Create "savings pots" for goals (e.g. holidays, emergency fund).
   - Create projects with a max budget to track targeted expenses.

C) 📈 INVESTMENTS
   - Record your investments (ETFs, stocks, crypto...).
   - Keep track of invested capital.

D) 📊 STATISTICS
   - Interactive charts: budget bars, % used, income vs expenses, top 5 expenses.
   - Generate and download PDF reports.
   - Export / import data, set spending limits.


3. HOW TO RECORD A TRANSACTION
--------------------------------

From the "Accounts" screen:

• + INCOME → Add money to an account (e.g. salary, refund).
• - EXPENSE → Subtract money from an account. Choose a category:
  - Essential (bills, groceries, fuel...)
  - Projects & Passions (hobbies, sport, creativity...)
  - Leisure / Extra (restaurants, cinema, shopping...)

You can link any expense to a Project to track its progress.


4. MULTIPLE ACCOUNTS
----------------------

You can create multiple accounts (e.g. Checking Account, Cash, PayPal, Revolut...).
Every transaction is tied to a specific account.

To create an account: tap "+ ACCOUNT" on the Accounts screen.
To edit or delete it: use the ✎ and × buttons next to the name.


5. RECURRING & SCHEDULED EXPENSES
-----------------------------------

🔄 RECURRING (Subscriptions)
   - Register recurring payments (Netflix, gym, rent...).
   - If you enter a "charge day" (1-31), the app records them
     automatically every month in the chosen account.
   - Without a charge day they stay manual: press "Add" when you pay.

📅 SCHEDULED
   - Enter future expenses with a due date (e.g. car tax, dentist).
   - The app warns you with a toast when 7 days or less remain.
   - When you actually pay, press the 💰 button to confirm the payment
     and register it as a real expense.


6. SAVINGS & PROJECTS
-----------------------

🏦 SAVINGS POTS
   - Create savings goals with a target amount.
   - Add money manually with the "ADD" button.
   - You can choose to deduct the amount from an account (automatically
     registering an expense in the "Savings" category).

🎯 PROJECTS
   - Ideal for works, trips or targeted purchases.
   - Assign a max budget: the progress bar turns red if you exceed it.
   - Expenses linked to the project are summed automatically.


7. INVESTMENTS
----------------

Register your financial assets to keep track of invested capital.
This value is separate from cash and savings.


8. STATISTICS & BUDGET
------------------------

In the "Statistics & Budget" screen you can:

• Filter by period: Week / Month / Year / All time.
• Choose the chart type:
  - Budget Bars: compare expenses by category against the set limit.
  - % Used: pie-chart distribution of expenses.
  - Income vs Expenses: period balance.
  - Top 5 Expenses: the heaviest outflows.

⚙️ SPENDING LIMITS (Budget)
   - Set a limit for each category (Essential, Passions, Leisure).
   - Each category has its own period: weekly, monthly or yearly.
   - When you reach 90% of the budget you get a toast alert.
   - If you exceed the limit the alert turns red.


9. PDF REPORTS
----------------

From the "Statistics & Budget" screen tap "📄 REPORT PDF" to generate
a professional financial report that you can download and share.

Available periods:
• This Week
• This Month
• Last 6 Months
• This Year

The PDF includes:
• Summary: total income, total expenses and net balance.
• Category Breakdown: how much you spent in each category with percentages.
• Monthly Trend: month-by-month income, expenses and net (if more than one month is covered).
• Current Account Balances: snapshot of all your accounts at the time of generation.

NOTE: the PDF is generated entirely on your device. The first time you use
this feature an internet connection is required to download the jsPDF library
from the CDN. After that it works offline too.


10. SETTINGS
--------------

Tap the gear icon ⚙️ in the top-right corner.

• 💱 Currency: switch between EUR, USD, GBP, CHF, JPY, CAD, AUD.
  All amounts are converted automatically using the current exchange rate
  (requires an internet connection).

• 🌍 Language: Italian / English.

• 🎨 Theme: Dark, Light, Ocean, Forest.

• 👁️ Privacy: toggle "privacy mode" to hide all sensitive figures
  (shows *** instead of amounts).

• 🔒 Auto-Lock: choose after how much inactivity the app asks for the PIN again.

• 🔐 PIN Protection: enable, disable or change the unlock PIN.


11. BACKUP & RESTORE
----------------------

💾 EXPORT
   - Download a JSON file with all your data.
   - If the PIN is active, the backup is also encrypted and protected.

📁 IMPORT
   - Load a previously exported JSON file.
   - If the backup is encrypted, you will be asked for the PIN used
     at the time of export.
   - The app warns you if the backup you are importing is older than the
     current data on the device.

🗑️ CLEAR HISTORY
   - Delete all transactions (income, expenses, savings...).
   - Account balances remain unchanged.
   - Useful for starting fresh without recreating accounts.


12. FAQ
---------

Q: Is my data safe?
A: Yes, it stays only on your device. If you enable the PIN it is encrypted
   with AES-256-GCM. No one (not even the developer) can access it.

Q: What happens if I clear browser data?
A: You lose everything. That's why regular JSON backups are essential.

Q: Can I use it offline?
A: Yes, except for currency conversion and the very first PDF generation
   which need internet to fetch external resources.

Q: Why don't I see browser notifications?
A: You must allow notifications when the browser asks.
   On iOS Safari web push notifications may be limited.

Q: I forgot my PIN. What do I do?
A: Tap "Forgot PIN?" on the lock screen.
   WARNING: this action deletes ALL data and resets the app.
   There is no way to recover data without the PIN.

Q: Can I edit a transaction after entering it?
A: Yes, tap the ✎ button next to the transaction in the list.
   You can change amount, description, account, category and project.


13. PRACTICAL TIPS
--------------------

1. Create your real accounts right away (Checking Account, Cash...).
2. Set monthly budgets to keep expenses under control.
3. Use Projects for important expenses (trips, renovations...).
4. Enable automatic recurring charges so you never forget a subscription.
5. Generate a PDF report before a meeting with your bank or accountant.
6. Export a JSON backup at least once a month.
7. If you use a PIN, write it down in a safe place (password manager).


Happy budgeting! 💰
