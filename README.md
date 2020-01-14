# banquepostale_to_csv

As La Banque Postale sucks and does not provide an easy way
to export data older than a few month in a usable format (ie. NOT pdf) I have created
this script to convert all the Banque Postale relevé in PDF to a CSV format.

I hope you'll find it useful

# Usage
`pdftotext` needs to be installed.
`pip install pdftotext --user`

On windows, pdftotext needs Microsoft Visual C++ 14.0.
1. Go to https://visualstudio.microsoft.com/downloads/ 
2. End of the page "Other Tools And Infrastructure"
3. Download Microsoft Visual C++ Redistributable For Visual Studio 2019
4. Install it, reboot the computer and retry to install pdftotext



Under linux you can install it by typing:
```shell
sudo apt-get install poppler-utils
```

To run the pdf to csv converter run:
```shell
python3 banquepostale_to_csv.py pdf_folder
```
where `pdf_folder` is the folder containing all the PDF relevés.
