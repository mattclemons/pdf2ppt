PDF to PowerPoint (pdf2ppt) Converter
pdf2ppt is a Python tool that converts each page of a PDF file into a separate slide in a PowerPoint presentation. This can be useful for presentations where you want to convert document pages into slides for easy viewing and editing.

Features
Convert PDF files into PowerPoint (.pptx) presentations.
Each page of the PDF becomes a separate slide in the PowerPoint file.
Prerequisites
This tool relies on the following libraries and tools:

Python 3.6+
pdf2image library for converting PDF pages to images.
Pillow library for image manipulation.
poppler for handling PDF conversions.
Installation
Clone the repository (if applicable):


git clone https://github.com/yourusername/pdf2ppt.git
cd pdf2ppt
Set up a virtual environment (recommended):


python3 -m venv venv
source venv/bin/activate  # On macOS/Linux
.\\venv\\Scripts\\activate   # On Windows
Install required Python packages:


pip install pdf2image Pillow python-pptx
Install Poppler (required by pdf2image):

macOS (using Homebrew):


brew install poppler
Linux (Debian/Ubuntu):


sudo apt update
sudo apt install poppler-utils
Windows:

Download Poppler for Windows from this link.
Extract the downloaded zip file, and add the path to poppler/bin to your system’s PATH environment variable.
Usage
Command-Line Interface
After setting up, you can use the script as follows:


python pdf2ppt.py <input_pdf_file> --output <output_pptx_file>
Options
<input_pdf_file>: Path to the PDF file you want to convert.
--output <output_pptx_file>: Path to save the converted PowerPoint file (e.g., output.pptx).
--help: Shows help and usage information.
Example
To convert document.pdf to presentation.pptx:


python pdf2ppt.py document.pdf --output presentation.pptx
Example Output
Each page of the PDF file will be converted into a slide within the specified PowerPoint file.

Troubleshooting
ModuleNotFoundError: No module named 'pdf2image': Ensure that you have installed the pdf2image library with pip install pdf2image.
OSError: poppler not found: Make sure Poppler is installed and accessible in your system's PATH. See the installation instructions above for details.
License
MIT License

This project was created to assist with automated PDF-to-PPTX conversions for presentation needs. Feel free to modify and improve the code as needed!

