# SeleniumVBA Excel Template

This template folder contains a minimal, ready-to-import copy of SeleniumVBA that can be reused in any Excel project.

## Contents

- `Modules/` – exported `.bas` and `.cls` files that make up SeleniumVBA.

## How to use the template in a new workbook

1. Download this `templates/ExcelTemplate` folder and unzip it anywhere on your machine.
2. Open your target workbook in Excel.
3. Press `ALT + F11` to open the VBA editor.
4. Import each file from `Modules/` (**File ▸ Import File…**) or drag the entire folder into the *VBAProject* window.
5. Ensure the required references are enabled. At a minimum you need:
   - Microsoft Scripting Runtime
   - Microsoft XML, v6.0
   - Microsoft HTML Object Library
   - Selenium Type Library (if using the add-in)
6. Save the workbook as a macro-enabled file (`.xlsm`).
7. Close and reopen Excel if prompted so that the WebDriver binaries can be downloaded automatically on first run.

## Updating the template

Whenever the core `src/VBA` modules change, copy the updated `.bas`/`.cls` files into `Modules/` (overwriting the existing copies) so the template always matches the main SeleniumVBA codebase.

