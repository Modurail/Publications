# Notes on Release 5.0
* It seemed wise to break out the various sections into separate files.

# Diagrams


# Other Images


# Pandoc Instructions
* Pandoc will create an output file of whichever type is needed (.docx, .html, etc.)
1. Install Pandoc on your local machine.
2. Pandoc is a command line tool only (no graphical interface), so go to the command prompt (for Windows use cmd.exe)
3. Navigate to the local file directory where the input files are.
4. The following command will create a standalone .docx file from the master .mmd file (no quotes): "pandoc -f markdown_mmd -t docx NGM_Master50.mmd -s -o NGM_Master50.docx --reference-docx=ngm-reference.docx"
5. Use a similar command to create other file types.

