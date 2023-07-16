# [Koinly](https://koinly.io) CSV Exporter

Download all your Koinly transaction to a single CSV file or multiple CSV files per wallet

## Warning!!
Running random scripts you find on the internet against authenticated accounts is generally a bad idea.  In this case it's safe; but you should thoroughly inspect the `script-single-csv.js` and `script-by-wallet-csv.js` file yourself before running it as a malicious script could result in account takeover, account deletion or other malicious activities.

## Steps
1. Login to your https://koinly.io account
2. Open Developer Tools on the Koinly app and select "Console" tab (It's done differently for Chrone, Safari & Edge so google how to open it for your browser if you're unsure)
3. Make a decision on what script you want to use
  * If you want to export all transaction at once into a single CSV file use `script-single-csv.js`
  * If you want to export multiple CSV files per wallet, use `script-by-wallet-csv.js`
4. Inspect the script for any malicious code (just generally good practice)
5. Copy the contents of your chosen script and paste it into the developer tools console; press enter
6. You should now be prompted for a path to save your transactions

## Customisation of of the CSV
1. Inspect the "console" output after running the script.  You will see the text "Your Koinly Transactions" printed.  Below this is all your transactions and all the information you have access to - you can click to expand it.  You are free to add any of this information to your CSV.
1. Search for `EXTRA_HEADERS` and `EXTRA_FIELDS` in the choses script file.  They explain where to add/remove entries.
