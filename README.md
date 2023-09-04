# Fix Henle PDF files for printing

The [Henle
application](https://play.google.com/store/apps/details?id=com.touchpress.henle)
for Android produces PDF files with wide margins.

To make them printable, the margin needs to be removed. This tool scales pages
of PDF with defaults to remove the margins of the Henle PDF.

The install steps you need to do the first time (some may be already done) are:

* Download and install git from https://git-scm.com/
* Download 3.11+ from [python.org](https://www.python.org/downloads/) and install
* Start command line and in it
* git clone https://github.com/kohtala/fixhenlepdf
* cd fixhenlepdf
* py -m venv .venv
* .venv\Scripts\activate
* pip install .

On subsequent times you need to

* Start command line, in it
* cd fixhenlepdf
* .venv\Scripts\activate

You can then change directory (cd) to where you have the PDF files to fix and

* py -m fixhenlepdf _the-original.pdf_

The printable PDF should appear in the same folder with the original with
`_print.pdf` suffix.
