#
# 📄 Table to CSV Exporter (Browser Console Script)

This project provides a lightweight JavaScript snippet that can be executed directly in the **browser console** to export the contents of an HTML `<table>` into a downloadable **CSV** file.

## 🚀 Features

- Automatically detects and processes the **first HTML table** on the page.
- Converts all rows and columns, including headers, into CSV format.
- Triggers a download of the CSV file named `Bisous.csv`.

## 🧠 How to Use

### Steps:

1. Navigate to the webpage containing the HTML table you want to export.
2. Open your browser’s **Developer Console**:
   - **Windows/Linux**: Press `F12` or `Ctrl + Shift + I`
   - **Mac**: Press `Cmd + Option + I`
3. Go to the **Console** tab.
4. Paste the following script and press **Enter**:


## To change the filename, modify this line in the script:

downloadLink.download = 'YourFileName.csv';
