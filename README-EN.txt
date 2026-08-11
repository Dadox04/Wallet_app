WALLET 5.5 — USER GUIDE
========================

A personal finance app that runs entirely in your browser.
All data stays on your device — no server, no cloud.


1. FIRST LAUNCH & SECURITY
----------------------------

On first open you can choose to enable a 4-digit PIN lock.

• PIN ON → data is encrypted with AES-256-GCM (PBKDF2) and stored securely.
  WARNING: if you forget the PIN there is no way to recover your data.
• PIN OFF → data is stored in plain text on the device.

Auto-lock: set a timer (1 / 5 / 15 / 30 minutes or "Never") after which the
app automatically locks if you stop using it or switch to another tab/app.
After 10 consecutive wrong attempts the keypad locks for 5 minutes.

If you forget your PIN, tap "Forgot PIN?" on the lock screen:
this action will PERMANENTELY erase all data and reset the app.


2. THE 4 MAIN SCREENS
---------------------

Navigate by swiping horizontally or tapping the bottom icons:

A) 💸 ACCOUNTS (Cash)
   - View total balance and account list.
   - Record income, expenses, recurring and scheduled payments.
   - Search recent transactions by description or category.

B) 🏦 PROJECTS (Savings)
   - Create "savings pots" for goals (e.g. holidays, emergencies).
   - Create projects with a max budget to track targeted spending.

C) 📈 INVESTMENTS
   - Record your assets (ETFs, stocks, crypto...).
   - Tracks invested capital separately from cash and savings.

D) 📊 STATISTICS
   - Interactive charts: budget bars, % used, income vs expenses, top 5 expenses.
   - Generate and download PDF and Excel reports.
   - Export / import data, set spending caps.


3. MULTIPLE ACCOUNTS
--------------------

Create as many accounts as you need (e.g. Checking, Cash, PayPal, Revolut...).
Every transaction is linked to a specific account.

To create an account: tap "+ ACCOUNT" on the Accounts screen.
To edit (name or balance) or delete: use the ✎ and × buttons.
At least one account must always remain active.


4. RECORDING A TRANSACTION
----------------------------

From the Accounts screen:

• + INCOME → Add money to an account (e.g. salary, refund).
• - EXPENSE → Deduct money from an account. Choose a category:
  - Essential (bills, groceries, fuel...)
  - Passions (hobbies, sports, creativity...)
  - Leisure / Extra (restaurants, cinema, shopping...)

You can link any expense to a Project to track its progress.


5. RECURRING & SCHEDULED EXPENSES
-----------------------------------

🔄 RECURRING (Subscriptions)
   - Register recurring payments (Netflix, gym, rent...).
   - If you set a "charge day" (1-31), the app records them automatically
     every month in the chosen account.
   - Without a charge day they stay manual: tap "Add" when you pay.

📅 SCHEDULED
   - Enter future expenses with a due date (e.g. car tax, dentist).
   - The app alerts you with a toast and, if allowed, a browser notification
     when 7 days or less remain (or if overdue).
   - When you pay, tap the 💰 button to confirm the payment and record it
     as an actual expense (you can adjust the amount on the fly).


6. SAVINGS & PROJECTS
---------------------

🏦 SAVINGS POTS
   - Create savings goals with a target amount.
   - Add money manually with the "ADD" button.
   - Choose whether to deduct the amount from an account (automatically
     recording a "Savings" category expense).
   - Tap ✎ to edit the name or target of an existing pot.

🎯 PROJECTS
   - Ideal for works, trips or targeted purchases.
   - Set a max budget: the progress bar turns red if you exceed it.
   - Expenses linked to the project are summed automatically.


7. INVESTMENTS
--------------

Record your financial assets to track invested capital.
This value is separate from cash and savings.
You can edit an existing investment by tapping the ✎ button.


8. STATISTICS & BUDGET
----------------------

On the "Statistics & Budget" screen you can:

• Filter by period: Week / Month / Year / All time.
• Choose chart type:
  - Budget Bars: compare spending per category against the set cap.
  - % Used: pie distribution of expenses.
  - Income vs Expenses: period balance.
  - Top 5 Expenses: your heaviest outflows.

⚙️ SPENDING CAPS (Budget)
   - Set a limit for each category (Essential, Passions, Leisure).
   - Each category has its own period: weekly, monthly or yearly.
   - When you reach 90% of the budget you get a toast alert.
   - If you exceed the limit the alert turns red.


9. PDF REPORT
-------------

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
• Monthly Trend: income, expenses and net month by month (if spanning >1 month).
• Current Account Balances: snapshot of all your accounts at generation time.

NOTE: the PDF is generated entirely on your device. The first time it needs
an internet connection to download the jsPDF library from CDN.
After that it works offline too.


10. EXCEL REPORT
----------------

Besides PDF you can export an Excel file with the full monthly historical
trend and an automatic 3-month forecast.

The file contains two sheets:
• Monthly Trend — summary of income, expenses per category, total expenses
  and net for every recorded month.
• Forecast — estimate for the next 3 months calculated with Excel FORECAST
  formulas (linear regression on historical data). If you have less than
  2 months of data the forecast is not yet available.

NOTE: the Excel export also needs internet the first time to load the
SheetJS library. After that it works offline.


11. EDITING & DELETING
----------------------

Made a mistake? No problem.

• Transactions: tap ✎ next to a transaction to change amount, description,
  account, category or linked project.
  WARNING: transactions older than one month are locked (🔒) and can no
  longer be edited or deleted, to keep your financial history reliable.
• Accounts: tap ✎ to rename an account or correct its balance.
• Savings pots: tap ✎ to edit name and target amount.
• Investments: tap ✎ to update name and capital.

Deleting a transaction automatically realigns the linked account balance.


12. SETTINGS
------------

Tap the gear icon ⚙️ in the top-right corner.

• 💱 Currency: switch between EUR, USD, GBP, CHF, JPY, CAD, AUD.
  All amounts are automatically converted using the current exchange rate
  (requires internet connection).

• 🌍 Language: Italiano / English.

• 🎨 Theme: Dark, Light, Ocean, Forest, Austere, Glacial.
  The last two (Austere and Glacial) use muted, cold colours specifically
  designed to reduce the urge to spend.

• 👁️ Privacy: enable "wink mode" to hide all sensitive figures
  (shows *** instead of amounts).

• 🔒 Auto-Lock: choose after how long of inactivity the app will ask
  for the PIN again (or "Never" to disable).

• 🔐 PIN Protection: enable, disable or change your unlock PIN.
  Changing the PIN does not require disabling protection first:
  enter your current PIN, then the new PIN twice.

• 🔔 Notifications: if you allow the browser, you will receive push
  notifications for upcoming scheduled expenses and exceeded budget alerts.

• 💾 / 📁 Export and Import data (see section 13).

Haptic feedback (light vibration on buttons) depends on your device's
system settings.


13. BACKUP & RESTORE
--------------------

💾 EXPORT
   - Download a JSON file with all your data.
   - If the PIN is active, the backup is also encrypted and protected.

📁 IMPORT
   - Load a previously exported JSON file.
   - If the backup is encrypted, you will be asked for the PIN used when
     the export was created.
   - The app warns you if the backup you are importing is older than the
     data currently on the device and asks for confirmation before overwriting.


14. FAQ
-------

Q: Is my data safe?
A: Yes, it stays only on your device. If you enable the PIN it is encrypted
   with AES-256-GCM. No one (not even the developer) can access it.

Q: What happens if I clear my browser data?
A: You lose everything. That's why regular JSON backups are essential.

Q: Can I use it offline?
A: Yes, except for currency conversion and the first PDF/Excel generation
   which need internet to fetch external libraries. After the first use
   both PDF and Excel work offline too.

Q: Why don't I see browser notifications?
A: You must allow notifications when the browser asks.
   On iOS Safari web push notifications may be limited.

Q: I forgot my PIN. What do I do?
A: Tap "Forgot PIN?" on the lock screen.
   WARNING: this will erase ALL data and reset the app.
   There is no way to recover data without the PIN.

Q: Can I edit a transaction after entering it?
A: Yes, tap the ✎ button next to the transaction in the list.
   You can change amount, description, account, category and project.
   Transactions older than one month are locked and cannot be edited.

Q: Why can't I delete an old expense?
A: To keep your financial history reliable, transactions recorded more than
   one month ago are automatically locked (🔒).

Q: The app vibrates when I tap buttons. Can I turn it off?
A: Haptic feedback depends on your device's system settings. If vibrations
   are enabled, the app uses them to confirm taps on main buttons.
