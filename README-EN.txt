WALLET 5.0 — USER GUIDE
================================

A personal finance app that runs entirely in your browser.
All your data stays on your device (no server, no cloud).


1. FIRST LAUNCH & SECURITY
----------------------------

On first open, you can choose whether to enable 4-digit PIN protection.

• PIN enabled → data is encrypted with AES-256-GCM and stored securely.
  WARNING: if you forget the PIN, there is no way to recover your data.
• PIN disabled → data is stored in plain text on your device.

Auto-lock: you can set a timer (1 / 5 / 15 / 30 minutes) after which
the app locks automatically if you stop using it or switch to another tab.

After too many failed attempts, the keypad locks for 5 minutes.


2. THE 4 MAIN SCREENS
-----------------------

Navigate by swiping horizontally or tapping the icons at the bottom:

A) 💸 ACCOUNTS (Cash)
   - View total balance and list of accounts.
   - Record income, expenses, recurring and scheduled payments.
   - Search recent transactions by description or category.

B) 🏦 PROJECTS (Savings)
   - Create "savings pots" for goals (e.g. holidays, emergencies).
   - Create projects with a max budget to track targeted spending.

C) 📈 INVESTMENTS
   - Record your investments (ETFs, stocks, crypto...).
   - Track invested capital.

D) 📊 STATISTICS
   - Interactive charts: budget bars, % used, income vs expenses, top 5 expenses.
   - Generate and download PDF and Excel reports.
   - Export / import data, set spending limits.


3. HOW TO RECORD A TRANSACTION
--------------------------------

From the "Accounts" screen:

• + INCOME → Add money to an account (e.g. salary, refund).
• - EXPENSE → Subtract money from an account. Choose the category:
  - Essential (bills, groceries, fuel...)
  - Passions (hobbies, sports, creativity...)
  - Leisure / Extra (restaurants, cinema, shopping...)

You can link any expense to a Project to track its progress.


4. MULTIPLE ACCOUNTS
----------------------

You can create multiple accounts (e.g. Checking, Cash, PayPal, Revolut...).
Every transaction is tied to a specific account.

To create an account: tap "+ ACCOUNT" on the Accounts screen.
To edit or delete it: use the ✎ and × buttons next to the name.
You can also correct an account's balance at any time.


5. RECURRING & SCHEDULED EXPENSES
-----------------------------------

🔄 RECURRING (Subscriptions)
   - Record recurring payments (Netflix, gym, rent...).
   - If you enter a "charge day" (1-31), the app records them
     automatically every month in the chosen account.
   - Without a charge day they remain manual: tap "Add" when you pay.

📅 SCHEDULED EXPENSES
   - Enter future expenses with a due date (e.g. car tax, dentist).
   - The app warns you with a toast and, if authorised, a browser
     notification when 7 days or less remain.
   - When you pay, tap the 💰 button to confirm the payment and
     record it as an actual expense (you can adjust the amount on the fly).


6. SAVINGS & PROJECTS
-----------------------

🏦 SAVINGS POTS
   - Create savings goals with a target amount.
   - Add money manually with the "ADD" button.
   - You can choose to deduct the amount from an account (automatically
     recording an expense in the "Savings" category).
   - Tap ✎ to edit the name or target of an existing pot.

🎯 PROJECTS
   - Ideal for jobs, trips or targeted purchases.
   - Assign a max budget: the progress bar turns red if you exceed the limit.
   - Expenses linked to the project are summed up automatically.


7. INVESTMENTS
----------------

Record your financial assets to track invested capital.
This value is separate from cash and savings.
You can edit an investment by tapping the ✎ button.


8. STATISTICS & BUDGET
------------------------

On the "Statistics & Budget" screen you can:

• Filter by period: Week / Month / Year / All time.
• Choose the chart type:
  - Budget Bars: compare expenses per category against the set limit.
  - % Used: pie-chart distribution of expenses.
  - Income vs Expenses: period balance.
  - Top 5 Expenses: the heaviest outflows.

⚙️ SPENDING LIMITS (Budget)
   - Set a limit for each category (Essential, Passions, Leisure).
   - Each category has its own period: weekly, monthly or yearly.
   - When you reach 90% of the budget you get a toast alert.
   - If you exceed the limit the alert turns red.


9. PDF REPORT
---------------

From the "Statistics & Budget" screen tap "📄 PDF REPORT" to generate
a professional financial report to download and share.

Available periods:
• This Week
• This Month
• Last 6 Months
• This Year

The PDF includes:
• Summary: total income, total expenses and net balance.
• Category Breakdown: how much you spent in each category with percentages.
• Monthly Trend: income, expenses and net month by month (if spanning more than one month).
• Current Account Balances: snapshot of all your accounts at generation time.

NOTE: the PDF is generated entirely on your device. The first time
an internet connection is needed to download the jsPDF library from CDN.
After that it works offline too.


10. EXCEL REPORT
------------------

Besides PDF you can export an Excel file with the complete monthly
historical trend and an automatic forecast for the next 3 months.

The file contains two sheets:
• Monthly Trend — summary of income, expenses by category, total outflows
  and net balance for every recorded month.
• Forecast — estimate for the next 3 months calculated with Excel FORECAST
  formulas (linear regression on historical data). If you have less than
  2 months of data, the forecast is not yet available.

NOTE: the Excel export also requires internet the first time to load
the SheetJS library. Afterwards it works offline.


11. EDITING TRANSACTIONS & ITEMS
----------------------------------

Made a mistake entering an expense? No problem.

• Transactions: tap ✎ next to a movement in the list to change
  amount, description, account, category or linked project.
• Accounts: tap ✎ to rename an account or correct its balance.
• Savings pots: tap ✎ to edit name and target amount.
• Investments: tap ✎ to update name and capital.

When you delete a transaction, the linked account balance is
automatically realigned.


12. SETTINGS
--------------

Tap the gear ⚙️ in the top right corner.

• 💱 Currency: switch between EUR, USD, GBP, CHF, JPY, CAD, AUD.
  All amounts are automatically converted using the current
  exchange rate (requires internet connection).

• 🌍 Language: English / Italiano.

• 🎨 Theme: Dark, Light, Ocean, Forest, Austere, Glacial.
  The last two (Austere and Glacial) use muted, cold colours
  specifically designed to reduce the urge to spend.

• 👁️ Privacy: enable "peek" mode to hide all sensitive figures
  (shows *** instead of amounts).

• 🔒 Auto-lock: choose after how long of inactivity the app
  asks for the PIN again (or "Never" to disable).

• 🔐 PIN Protection: enable, disable or change the unlock PIN.
  Changing the PIN does not require disabling protection first:
  enter the current PIN, then the new PIN twice.

• 🔔 Notifications: if you authorise the browser, you will receive
  push notifications for upcoming scheduled expenses and budget alerts.


13. BACKUP & RESTORE
----------------------

💾 EXPORT
   - Download a JSON file with all your data.
   - If the PIN is active, the backup is also encrypted and protected.

📁 IMPORT
   - Load a previously exported JSON file.
   - If the backup is encrypted, you will be asked for the PIN used
     at the time of export.
   - The app warns you if the backup you are importing is older than
     the data currently on the device.

🗑️ CLEAR HISTORY
   - Delete all movements (income, expenses, savings...).
   - Account balances remain unchanged.
   - Useful for starting fresh without recreating accounts.


14. FREQUENTLY ASKED QUESTIONS
--------------------------------

Q: Is my data safe?
A: Yes, it stays only on your device. If you enable the PIN it is encrypted
   with AES-256-GCM. No one (not even the developer) can access it.

Q: What happens if I clear browser data?
A: You lose everything. That's why regular JSON backups are essential.

Q: Can I use it offline?
A: Yes, except for currency conversion and the first PDF/Excel generation
   which need internet to fetch external resources.

Q: Why don't I see browser notifications?
A: You must authorise notifications when the browser asks.
   On iOS Safari web push notifications may be limited.

Q: I forgot my PIN. What do I do?
A: Tap "Forgot PIN?" on the lock screen.
   WARNING: this action deletes ALL data and resets the app.
   There is no way to recover data without the PIN.

Q: Can I edit a transaction after entering it?
A: Yes, tap the ✎ button next to the movement in the list.
   You can change amount, description, account, category and project.

Q: The app vibrates when I tap buttons. Can I turn it off?
A: Haptic feedback depends on your device's system settings. If vibrations
   are enabled, the app uses them to confirm taps on main buttons.


15. PRACTICAL TIPS
--------------------

1. Create your real accounts right away (Checking, Cash...).
2. Set monthly budgets to keep spending under control.
3. Use Projects for big expenses (trips, renovations...).
4. Enable Recurring Expenses with auto-charge so you never forget
   a subscription.
5. Generate a PDF report before a meeting with your bank or accountant.
6. Export the Excel report to analyse trends and forecasts
   directly in a spreadsheet.
7. Export a JSON backup at least once a month.
8. If you use a PIN, write it down in a safe place (password manager).


Happy budgeting! 💰
