# PDF_Text_Extraction
This repository provides efficient Python scripts for extracting text from PDF files and converting it into a JSON line format for easy storage and further processing. The extraction process is implemented using two different methods, leveraging the power of Python libraries PyMuPDF and Grobid.

Methods:
PyMuPDF Method: The repository includes a robust script utilizing the PyMuPDF library, which offers high-performance PDF parsing and text extraction capabilities. This method ensures accurate extraction of text content from PDF files, enabling you to process and store the data efficiently.
Grobid Method: Additionally, this repository offers an alternative script that utilizes the Grobid library for PDF text extraction. Grobid is a powerful tool specifically designed for extracting structured information from scholarly documents. This method provides an alternative approach with its unique set of features, ensuring flexibility in extracting text from PDF files.

Benefits:
Simplifies PDF text extraction: The provided scripts eliminate the complexity of extracting text from PDF files, allowing you to focus on leveraging the extracted content for your specific use cases.
JSON line format: The extracted text is converted into a JSON line format, providing a structured and easily manageable representation for storage and further processing.
Two methods for flexibility: The availability of two different extraction methods, PyMuPDF and Grobid, offers flexibility in choosing the approach that best suits your requirements.


You need docker to run the grobid image on:

*****Pulling the grobid into docker*****
docker pull grobid/${version}
docker pull grobid/grobid:0.8.0

*****Starting the docker image*****
docker run --rm --init --ulimit core=0 -p 8070:8070 grobid/grobid:0.8.0

*****After starting check if server if up*****
http://localhost:8070

*****Also refer to*****
Note: Please make sure to refer to the documentation and licensing of the PyMuPDF and Grobid libraries for any specific usage guidelines or restrictions.
Official Documentation - https://grobid.readthedocs.io/en/latest/Principles/
Grobid Repository - https://github.com/kermitt2/grobid_client_python
