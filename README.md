# Fix Henle PDF files for printing

The [Henle
application](https://play.google.com/store/apps/details?id=com.touchpress.henle)
for Android produces PDF files with wide margins.

To make them printable, the margin needs to be removed. This tool scales pages
of PDF with defaults to remove the margins of the Henle PDF.

To install this tool, I assume you have already cloned this source and are in
the folder with this `README.md`.

* Install Python (3.11 or newer) with PIP
* Create virtual environment
* Activate the virtual environment
* Install this source code in the virtual environment
* Run the tool

I assume you have already cloned this source On Windows this is in practice

* Download from [python.org](https://www.python.org/downloads/) and install
* py -m venv .venv
* .venv\Scripts\activate
* pip install .
* python -m fixhenlepdf _the-original.pdf_

The printable PDF should appear in the same folder with the original with
`_print.pdf` suffix.
