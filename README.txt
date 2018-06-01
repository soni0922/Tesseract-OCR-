Tesseract OCR Package Behavior: 

1) 'main.exe' , tessdata folder and all dll's should be present in one folder.
2) Run main.exe in the following manner : 

	PS main.exe inputImageFileFullPath outputFileFullPath

3) outputFileFullPath is optional. If it is not specified, the output csv file is written into the input source file path with the same name as image file name.
4) Necessary warnings/errors are produced in erroneous situations. For example:
	 PS main.exe C:\Users\testImage.png
	    Cannot open input file: C:\Users\testImage.png
5) English training data is included in tessdata folder
6) The first row which depicts the image height and width is not being produced in the output csv file.