
A lightweight two-part toolset to extract HTML table data into CSV format via the browser, and then generate a styled Excel report from that CSV.

---

## PART 01: Table to CSV Exporter (JavaScript - Browser Console)

This JavaScript snippet can be run directly in your **browser's developer console** to export the contents of the first `<table>` element on a webpage into a downloadable **CSV** file.

### 🚀 Features

- Automatically detects and processes the **first HTML table** on the page.
- Converts all rows and columns, including headers, into CSV format.
- Triggers a download of a file named `Bisous.csv`.

### 🧠 How to Use

1. Navigate to the webpage containing the HTML table.
2. Open your browser’s **Developer Console**:
   - **Windows/Linux**: `F12` or `Ctrl + Shift + I`
   - **Mac**: `Cmd + Option + I`
3. Go to the **Console** tab.
4. Paste the provided JavaScript snippet and press **Enter**.

> 💡 To change the filename, modify this line in the script:
```javascript
downloadLink.download = 'YourFileName.csv';
```

---

## PART 02: CSV to Excel Report Generator (Python)

This Python script reads the `Bisous.csv` file and generates a clean, styled Excel report that highlights **redundant services per host**.

### 🚀 Features

- Reads a semicolon-separated CSV file.
- Counts how many times each service appears per host.
- Filters only services that appear **more than once** per host.
- Outputs a styled Excel file named: `REDONDANT ALERT PELATRO.xlsx`.

### 📦 Requirements

Install the required Python packages:

```bash
pip install pandas openpyxl
```

### 🧠 How to Use

1. Make sure `Bisous.csv` is in the same directory as the script.
2. Run the script:

```bash
python generate_excel_report.py
```

3. The script will generate a file named `REDONDANT ALERT PELATRO.xlsx`.

---

### 📁 Output Example

The generated Excel file includes:

- **Bold white headers** on a **blue background**
- **Auto-adjusted column widths**
- **Centered header text**

---

### 🛠️ Customization

- **Change the output filename**:
```python
wb.save('YourFileName.xlsx')
```

- **Adjust the redundancy threshold**:
```python
if count > 1  # Modify this value as needed
```

---

## 📬 Contact

For questions, suggestions, or contributions, feel free to open an issue or submit a pull request!

---
```
