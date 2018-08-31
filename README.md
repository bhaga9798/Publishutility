# Publishutility
Installation files for Port Monitor and Ghostscript which are essential for creating a Printer to generate PDF Files.
Note: Ghostscript for all platforms can be downloaded from https://github.com/ArtifexSoftware/ghostpdl-downloads/releases/download/gs923/gs923w64.exe
1. In Windows, go to the Add Printer Wizard. (Settings-->Printers and Scanners)
2. Click “Your Printer has not been listed” 
3. In the Window that appears, select the option “Add a Local Printer or Network Printer with Manual Settings”. In the next window that appears, select “Create A New Port” and select Multifile Port Monitor from the dropdown list.
4. You’ll get the above window. Enter a output path for your PDF File. You can have  a specified pattern for the files. Click on the help icon to know more about the  naming patterns.  
5. In the User Command, enter the following ghostscript command. 
6. “C:\Program Files\gs\gs9.21\bin\gswin64c.exe" -dBATCH -dSAFER -dNOPAUSE -sDEVICE=pdfwrite -dPDFSETTINGS=/prepress -dAutoRotatePages=/PageByPage -r600 -sOutputFile="%f" - 
NOTE: The location should be the storage where ghostscript has been installed​.  6. Leave the rest of the settings as default and click OK. 
7. The “Add Printer” wizard shows up again for selecting the drivers. Select any of  your preferred Postscript Printer Drivers. Ghostscript has provided a postscript  printer driver by themselves.  
8. Now, the PDF Printer is all ready. 
9. The PDF File generated can be further enhanced by using specific ghostscript  commands.  
