WALLET 6.0 — USER GUIDE
=======================

A personal finance app that runs directly in your browser.
All data stays on your device (no server, no cloud).


1. FIRST LAUNCH & SECURITY
----------------------------

On first launch you can choose whether to enable 4-digit PIN protection.

• PIN ON → data is encrypted with AES-256-GCM (PBKDF2) and stored
  securely on the device.
  WARNING: if you forget the PIN there is no way to recover the data.
• PIN OFF → data remains unencrypted on the device.

Auto-lock: you can set a timer (1 / 5 / 15 / 30 minutes or "Never")
after which the app automatically locks if you stop using it or switch to
another tab/app. After 10 consecutive wrong attempts the keypad is locked
for 5 minutes.

If you forget the PIN, tap "Forgot PIN?" on the lock screen:
this action will PERMANENTLY delete all data and reset the app.


2. THE 4 MAIN SCREENS
-----------------------

Navigate by swiping horizontally or tapping the icons at the bottom:

A) 💸 ACCOUNTS (Cash & Accounts)
   - View total balance and list of accounts.
   - Record income, expenses, recurring and scheduled expenses.
   - Search recent transactions by description or category.

B) 🏦 PROJECTS (Savings & Projects)
   - Create "savings pots" for goals (e.g. holidays, emergencies).
   - Create projects with a maximum budget to track targeted expenses.

C) 📈 INVESTMENTS
   - Register your investments (ETFs, stocks, crypto...).
   - Keeps track of invested capital.

D) 📊 STATS & BUDGET
   - Interactive charts: budget bars, % used, income vs expenses, top 5 expenses.
   - Generate and download PDF and Excel reports.
   - Export / import data, set spending limits.


3. MULTIPLE ACCOUNTS
--------------------

You can create multiple accounts (e.g. Checking, Cash, PayPal, Revolut...).
Every transaction is linked to a specific account.

To create an account: tap "+ ACCOUNT" on the Accounts screen.
To edit (name or balance) or delete: use the ✎ and × buttons.
At least one account must always remain active.


4. HOW TO RECORD A TRANSACTION
--------------------------------

From the "Accounts" screen:

• + INCOME → Add money to an account (e.g. salary, refund).
• - EXPENSE → Subtract money from an account. Choose a category:
  - Essential (bills, groceries, fuel...)
  - Passions (hobbies, sports, creativity...)
  - Leisure / Extra (restaurants, cinema, shopping...)

You can link every expense to a Project to track its progress.


5. RECURRING & SCHEDULED EXPENSES
-----------------------------------

🔄 RECURRING EXPENSES (Subscriptions)
   - Register recurring payments (Netflix, gym, rent...).
   - If you enter a "charge day" (1-31), the app records them
     automatically every month in the chosen account.
   - Without a charge day they remain manual: press "Add" when you pay.
   - You can link every recurring expense to a Project.

📅 SCHEDULED EXPENSES
   - Enter future expenses with a due date (e.g. car tax, dentist).
   - The app alerts you with a toast and, if authorised, with a browser
     notification when 7 days or fewer remain (or if overdue).
   - When you pay, press the 💰 button to confirm the payment and
     record it as an actual expense (you can adjust the amount on the fly).
   - You can link every scheduled expense to a Project.


6. SAVINGS & PROJECTS
-----------------------

🏦 SAVINGS POTS
   - Create savings goals with a target amount.
   - Add money manually with the "ADD" button.
   - You can choose whether to deduct the amount from an account (automatically
     recording an expense in the "Savings" category).
   - Tap ✎ to edit the name or target of an existing pot.

🎯 PROJECTS
   - Ideal for works, trips or targeted purchases.
   - Assign a maximum budget: the progress bar turns red if you exceed the limit.
   - Expenses linked to the project are summed automatically.
   - Deleting a project keeps already recorded expenses in the general history.


7. INVESTMENTS
----------------

Register your financial assets to keep track of invested capital.
This value is separate from cash and savings.
You can edit an existing investment by tapping the ✎ button.


8. STATISTICS & BUDGET
------------------------

On the "Stats & Budget" screen you can:

• Filter by period: Week / Month / Year / All time.
• Choose the chart type:
  - Budget Bars: compare expenses by category against the set limit.
  - % Used: pie-chart distribution of expenses.
  - Income vs Expenses: period balance.
  - Top 5 Expenses: the heaviest outflows.

⚙️ SPENDING LIMITS (Budget)
   - Set a limit for each category (Essential, Passions, Leisure).
   - Each category has its own period: weekly, monthly or yearly.
   - When you reach 90% of the budget a toast alert is shown.
   - If you exceed the limit the alert turns red.


9. PDF REPORT
---------------

From the "Stats & Budget" screen tap "📄 PDF REPORT" to generate
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
• Current Account Balances: snapshot of all your accounts at the time of generation.

NOTE: the PDF is generated entirely on your device. The first time
an internet connection is required to download the jsPDF library from CDN.
After that it works offline as well.


10. EXCEL REPORT
-----------------

In addition to PDF you can export an Excel file with the complete monthly
historical trend and an automatic forecast for the next 3 months.

The file contains two sheets:
• Monthly Trend — summary of income, expenses by category, total expenses
  and net for every recorded month.
• Forecast — estimate for the next 3 months calculated with Excel FORECAST
  formulas (linear regression on historical data). If you have fewer than
  2 months of data the forecast is not yet available.

NOTE: the Excel export also requires internet the first time to load
the SheetJS library. After that it works offline.


11. EDITING & DELETING
------------------------

Made a mistake entering an expense? No problem.

• Transactions: tap ✎ next to a transaction in the list to change
  amount, description, account, category or linked project.
  WARNING: transactions recorded more than a month ago are locked
  (🔒) and can no longer be edited or deleted, to ensure the reliability
  of the historical record.
• Accounts: tap ✎ to rename an account or correct its balance.
• Savings pots: tap ✎ to edit name and target amount.
• Investments: tap ✎ to update name and capital.

Deleting a transaction automatically realigns the balance of the linked account.


12. SETTINGS
--------------

Tap the gear ⚙️ icon at the top right.

• 💱 Currency: switch between EUR, USD, GBP, CHF, JPY, CAD, AUD.
  All amounts are automatically converted using the current exchange rate
  (requires internet connection).

• 🌍 Language: Italian / English.

• 🎨 Theme: Dark, Light, Ocean, Forest, Austere, Glacial.
  The last two (Austere and Glacial) use muted and cold colours
  specifically designed to reduce the urge to spend.

• 👁️ Privacy: enable "peek" mode to hide all sensitive figures
  (shows *** instead of amounts).

• 🔒 Auto-lock: choose after how long of inactivity the app asks
  for the PIN again (or "Never" to disable).

• 🗄️ History Retention: choose how long to keep the full transaction detail
  (Never, 6 months, 1 year, 2 years, 3 years, 5 years).
  Older transactions are compacted into monthly category totals
  (still available in PDF/Excel reports) and then removed in detail
  to keep the file lightweight. This operation cannot be undone.

• 🔐 PIN Protection: enable, disable or change the unlock PIN.
  Changing the PIN does not require disabling protection first:
  enter the current PIN, then the new PIN twice.

• 🔔 Notifications: if you authorise the browser, you will receive push
  notifications for upcoming scheduled expenses and budget limit alerts.

• 💾 / 📁 Export and Import data (see section 13).

Haptic feedback (light vibration on buttons) depends on your device's
system settings.


13. BACKUP & RESTORE
----------------------

💾 EXPORT
   - Download a JSON file with all your data.
   - If PIN is active, the backup is also encrypted and protected.

📁 IMPORT
   - Load a previously exported JSON file.
   - If the backup is encrypted, you will be asked for the PIN used
     at the time of export.
   - The app warns you if the backup you are importing is older than
     the current data on the device and asks for confirmation before overwriting.


14. FREQUENTLY ASKED QUESTIONS
--------------------------------

Q: Is my data safe?
A: Yes, it stays only on your device. If PIN is enabled it is encrypted
   with AES-256-GCM. No one (not even the developer) can access it.

Q: What happens if I clear browser data?
A: You lose everything. That's why regular JSON backups are essential.

Q: Can I use it offline?
A: Yes, except for currency conversion and the first PDF/Excel generation
   which require internet to fetch external resources. After first use
   both PDF and Excel work offline.

Q: Why don't I see browser notifications?
A: You must authorise notifications when the browser prompts you.
   On iOS Safari web push notifications may be limited.

Q: I forgot the PIN. What do I do?
A: Tap "Forgot PIN?" on the lock screen.
   WARNING: this action deletes ALL data and resets the app.
   There is no way to recover the data without the PIN.

Q: Can I edit a transaction after entering it?
A: Yes, tap the ✎ button next to the transaction in the list.
   You can change amount, description, account, category and project.
   Transactions older than one month are locked and cannot be edited.

Q: Why can't I delete an old expense?
A: To keep the financial history reliable, transactions recorded
   more than a month ago are automatically locked (🔒).

Q: The app vibrates when I tap buttons. Can I turn it off?
A: Haptic feedback depends on your device's system settings.
   If vibrations are enabled, the app uses them to confirm every tap
   on the main buttons.
