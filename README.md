# Fix Henle PDF files for printing

The [Henle
application](https://play.google.com/store/apps/details?id=com.touchpress.henle)
for Android (at time of writing version 1.9.1) produces PDF files with wide margins.

To make them more readable when printed, the margin needs to be removed. This
tool scales pages of PDF with defaults to remove the margins of the Henle PDF.

The install steps you need to do the first time (some may be already done) are:

* Install Python
  * On Windows from [python.org](https://www.python.org/downloads/) or from store
  * On Linux you most likely have it already or install using package manager
* Start command prompt and execute in it command
* pip install git+https://github.com/kohtala/fixhenlepdf.git

You can then change directory (`cd`) to where you have the PDF files to fix
and on Windows

    py -m fixhenlepdf _the-original.pdf_

or if `pip install` did not display a warning that the `fixhenlepdf` is not on
`PATH` simply

    fixhenlepdf _the-original.pdf_

The printable PDF should appear in the same folder with the original with
`_print.pdf` suffix.

On-line help is available with `--help` option.
