# Optical-Character-Recognition

OCR (optical character recognition) is the recognition of printed or written text characters by a computer.

In order to perform OpenCV OCR text recognition, we’ll first need to install Tesseract v4 which includes a highly accurate deep learning-based model for text recognition.

## Dependencies ##

* Pytesseract
* OpenCV
* Numpy

## Technique ##

* To start, we’ll apply OpenCV’s EAST text detector to detect the presence of text in an image. The EAST text detector will give us the bounding box (x, y)-coordinates of text ROIs.

* We’ll extract each of these ROIs and then pass them into Tesseract v4’s LSTM deep learning text recognition algorithm.

* The output of the LSTM will give us our actual OCR results.

* Finally, we’ll draw the OpenCV OCR results on our output image.
