# Tesseract

Pytesseract or Python-tesseract is an Optical Character Recognition (OCR) tool for Python. 
It will read and recognize the text in images, license plates etc. 
Python-tesseract is actually a wrapper class or a package for Google’s Tesseract-OCR Engine. 
It is also useful and regarded as a stand-alone invocation script to tesseract, 
as it can easily read all image types supported by the Pillow and Leptonica imaging libraries, which mainly includes –
jpg
png
gif
bmp
tiff etc



Installtion:

Installing via pip:

Check the pytesseract package page for more information.

     pip install pytesseract

Or if you have git installed:
                                                   
     pip install -U git+https://github.com/madmaze/pytesseract.git

Installing from source:
    
     git clone https://github.com/madmaze/pytesseract.git
      
     cd pytesseract && pip install -U .

Install with conda (via conda-forge):

     conda install -c conda-forge pytesseract
     
     
    
    
Functions:

     get_languages-->Returns all currently supported languages by Tesseract OCR.
     get_tesseract_version-->Returns the Tesseract version installed in the system.
     image_to_string--> Returns unmodified output as string from Tesseract OCR processing
     image_to_boxes--> Returns result containing recognized characters and their box boundaries
     image_to_data--> Returns result containing box boundaries, confidences, and other information. Requires Tesseract 3.05+. For more information, please check the       Tesseract TSV documentation
     image_to_osd--> Returns result containing information about orientation and script detection.
     image_to_alto_xml--> Returns result in the form of Tesseract's ALTO XML format.
     run_and_get_output--> Returns the raw output from Tesseract OCR. Gives a bit more control over the parameters that are sent to tesseract.
