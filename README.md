# Pocket Budget

A free, private budget app in one HTML file. No server, no sign-up. Drop in CSV exports from your banks and it works out each file's columns, date format, signs and currency. It sorts transactions into categories, remembers your fixes as rules, pairs card payments between your own accounts as transfers, and shows income, spending against a budget, and what's left each month. Everything stays in your browser, and the page blocks all network requests.

Use it: https://denzil10.github.io/pocket-budget/

Built by an AI agent (Claude Code) from one prompt in 8m 29s, then fixed after a British bank file broke it (5m 38s). Shown on the YouTube channel Agent at Work (@theagentatwork).

- `index.html`: the app after the fix (day-first dates, a currency per account).
- `first-build/index.html`: the first build, before the fix. It reads 03/11/2026 as March 11 in a US-English browser.
- `samples/`: made-up statements in the layouts of Capital One, Chase, Amex, Bank of America, a headerless checking export, and Barclays. No real data.

Known limit: a file with no currency clue at all (no symbol, sort code, IBAN or known bank layout) falls back to your browser's language for currency and shows a "Check the currency" warning.
