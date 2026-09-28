# CIS-team-project

A Python-based GUI application designed to parse unstructured court text documents (`.txt`) and convert them into formatted, analyzable Excel spreadsheets (`.xlsx`).

## Features
* **Modern GUI:** Built with `ttkbootstrap` for a clean "Minty" themed interface.
* **Batch Processing:** Select and process up to 3 text files simultaneously.
* **Data Extraction:** Automatically parses dates, case numbers, defendant names, attorneys, charges, pleas, and bond information using RegEx.
* **Excel Export:** Outputs data to `Court_Output.xlsx` with auto-formatted tables.
* **Auto-Launch:** Option to automatically open the resulting Excel file upon completion.

## Prerequisites

* Python 3.x installed on your system.

## Installation

1.  **Clone or Download** this repository to your local machine.
2.  **Install Dependencies:**
    Open your terminal or command prompt and run the following command to install the required libraries (`pandas`, `xlsxwriter`, and `ttkbootstrap`):

    ```bash
    pip install pandas xlsxwriter ttkbootstrap
    ```

    *Alternatively, if a requirements.txt file is provided:*
    ```bash
    pip install -r requirements.txt
    ```

## Usage

1.  Run the application:
    ```bash
    python group_projectGUIv1.py
    ```

2.  Click **Browse** to select your court text files (File 1, File 2, or File 3).
3.  Click **PROCESS DATA**.
4.  Once finished, the application will ask if you want to open the generated Excel file.

## Troubleshooting

* **Permission Error:** If you have `Court_Output.xlsx` open in Excel while trying to run the script, the program will fail to save. Please close the Excel file and try again.
* **No Data Found:** Ensure your text files match the expected format (Header, Court Date patterns, etc.) required by the internal Regex parsers.

## Credits

* **Co-written with https://github.com/Toweryjg502**
