Transaction Receipt Generation


This project demonstrates how to generate a PDF receipt using Python's ReportLab library. The generated PDF includes a table displaying transaction 
details such as date, item name, subscription type, and price, along with a subtotal, discount, and total amount.

Table of Contents

Installation

Usage

Code Explanation

License

Installation

To run this script, you need to have Python installed on your system along with the ReportLab library. If you don't have ReportLab installed, you can install it using pip:
pip install reportlab

Usage
Clone this repository or download the script file to your local machine.
Run the Python script using the following command:
python generate_receipt.py
This will generate a PDF file named receipt.pdf in the same directory as the script.

Code Explanation
The script uses the ReportLab library to create a PDF document with the following components:

Imports: The necessary modules from ReportLab are imported for creating the document, table, styles, and colors.

Data Definition: A list named DATA is defined, containing the transaction details that will be displayed in the PDF table.

PDF Template Creation: A SimpleDocTemplate is created to define the base template for the PDF. The pagesize is set to A4.

Stylesheet and Title: The default stylesheet is obtained using getSampleStyleSheet(). A title for the PDF, "Bits & Bites", is created with the Heading1 style and centered alignment.

Table Style: The TableStyle class is used to define the appearance of the table, including borders, grid lines, background colors, text color, and alignment.

Table Creation: A Table object is created with the defined data and style.

PDF Generation: The build method of the SimpleDocTemplate is called with the title and table objects to generate the final PDF document.

License
This project is licensed under the MIT License. See the LICENSE file for more details.
