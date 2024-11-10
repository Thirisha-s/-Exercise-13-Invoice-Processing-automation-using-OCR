## Exercise_13-Invoice_Processing_automation_using_OCR
```
Name: THIRISHA S
Reg No: 212222230160
```
## Aim:

To automate the extraction of specific data (Invoice Number, Date, and Total Amount) from an invoice PDF using OCR and store the extracted information in an Excel file.

## Equipments Required:

UiPath Studio<br>
Invoice PDF file<br>
Excel file for storing extracted data<br>

#### Installed UiPath packages:

UiPath.PDF.Activities<br>
UiPath.IntelligentOCR.Activities<br>
UiPath.Excel.Activities<br>

## Procedure:

### Install UiPath and Required Packages:

Download and install UiPath Studio.<br>
Create a new project and install the necessary packages (PDF, OCR, Excel).<br>

### Read the Invoice PDF with OCR:

Use the Read PDF with OCR activity to extract text from the PDF.<br>
Choose an OCR engine like Tesseract to process the document.<br>

### Extract Specific Data Using Regex:

Add the Matches activity to extract the Invoice Number, Date, and Total Amount using regular expressions:<br>
Invoice Number: INV-\d+<br>
Date: \d{2}/\d{2}/\d{4}<br>
Total Amount: \₹?\d+(,\d{3})\*(\.\d{2})?<br>
Store the extracted values in variables.<br>

### Write Data to Excel:

Use the Excel Application Scope activity to open or create an Excel file.<br>
Write the extracted data (Invoice Number, Date, Total Amount) into specific cells using Write Cell activity.<br>

### Run and Test:

Run the workflow and verify that the data has been extracted correctly and saved into the Excel file.

## UiPath WorkFlow:
![Screenshot 2024-10-12 202115](https://github.com/user-attachments/assets/292aa64f-4390-4a6d-9c35-0988291537b3)
![Screenshot 2024-10-12 203929](https://github.com/user-attachments/assets/e1f30f11-b1a4-404b-86cb-53e0a59e31c8)
![Screenshot 2024-10-12 204423](https://github.com/user-attachments/assets/c8ab0ac7-a67b-4ac7-92f5-331ef2b9cd42)
![Screenshot 2024-10-12 204452](https://github.com/user-attachments/assets/7bcad99f-91e0-456f-8a1b-b0ca8da188f2)
![Screenshot 2024-10-12 205632](https://github.com/user-attachments/assets/936ae8f8-4a0e-4e39-84a8-4b152ca4a3a9)
![Screenshot 2024-10-12 205752](https://github.com/user-attachments/assets/730a5a68-cfb7-4500-b8a2-2c9add065dc4)
![Screenshot 2024-10-12 210327](https://github.com/user-attachments/assets/a76069fd-3134-4f53-891b-04e5ec01b467)

## Result:

The automation successfully extracts the Invoice Number, Date, and Total Amount from the PDF and enters them into an Excel file, demonstrating efficient invoice processing using OCR.
