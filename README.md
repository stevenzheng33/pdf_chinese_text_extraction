# PDF Chinese Text Extraction
## Overview
The script converts pdf to jpegs and then use OCR to recognize all the Chinese characters


## Features
- Import pdf and export text only
- Use open-source packages
- Allows for offline processing
- Easy to incorporate regex expression


## Packages Required
- [pdf2image](https://pypi.org/project/pdf2image/)
- [PIL](https://pillow.readthedocs.io/en/stable/)
- [pytesseract](https://pypi.org/project/pytesseract/)
- Download the simplified Chinese package from the github [repo](https://github.com/tesseract-ocr/tessdata/raw/master/chi_sim.traineddata) and add it in the **tessdata** folder.


## How to use

- Save the pdfs into a folder under the script directory.
- Run the script.py and input the directory as the variable.
- Save the result string for future processing.

## Regex Keywording

The script automatically processes the string by getting rid of the empty space and newline characters. It combines the text from multiple pages and puts them into one. One important way to extract the data is to use regular expression to locate the information. Use function such as findall to locate the keyword and snoop around to find the number or textual information.
