### pdf2ppt is a Python tool that converts each page of a PDF file into a separate slide in a PowerPoint presentation.

    git clone https://github.com/yourusername/pdf2ppt.git && cd pdf2ppt 

### Install Poppler (required by pdf2image):

### macOS (using Homebrew):

    brew install poppler

### Linux (Debian/Ubuntu):

    sudo apt update sudo apt install poppler-utils 

### Set up a virtual environment (recommended):

    python3 -m venv venv 
    source venv/bin/activate
    pip install pdf2image Pillow python-pptx         

### Use the script as follows:

    python pdf2ppt.py <input_pdf_file> --output <output_pptx_file>


### --help: Shows help and usage information. Example To convert document.pdf to presentation.pptx:

    python pdf2ppt.py document.pdf --output presentation.pptx
