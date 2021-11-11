# Notes on Release 5.2
* The only change is from unregulated 16 VDC to regulated 12 VDC accessory power.

# Pandoc Instructions
* Pandoc will create an output file of whichever type is needed (.docx, .html, etc.)
1. Install Pandoc on your local machine.
2. Pandoc is a command line tool only (no graphical interface), so go to the command prompt (for Windows use cmd.exe)
3. Navigate to the local file directory where the input files are.
4. The following command will create a standalone .docx file from the master .mmd file (no quotes): "pandoc -f markdown_mmd -t docx NGM_Master52.mmd -s -o NGM_Master52.docx --reference-docx=ngm-reference.docx"
5. Use a similar command to create other file types.

# Release 5.2 Final Production
* Date: Set when complete.

* Updated electrical reference for 16VDC to 12VDC.

## Step 1: Create docx file.
1. Used the following pandoc command to generate the initial docx file (no quotes): `pandoc --from=markdown_mmd --to=docx Title52.mmd Introduction52.mmd Electrical52.mmd Trackwork52.mmd Framework52.mmd Scenery52.mmd Diagrams52.mmd Definitions52.mmd Revisions52.mmd --reference-doc=ngm-reference2.docx -s -o "NGM Module Specifications 52.docx" `

2. Cleaned up the output file:

    1. Edited a document property, `Document number` as 5.2 (this is referenced in the document footer).
    
    2. Made a few pagination adjustments.
    
    3. Inserted an auto-TOC.

## Step 2: Create PDF
Created the PDF as an export from the docx file.

## Step 3: Create HTML
Used this Pandoc command to generate the HTML version (no quotes): `pandoc -s -N -c tufte.css --from=markdown_mmd --to=html --toc Title52.mmd Introduction52.mmd Electrical52.mmd Trackwork52.mmd Framework52.mmd Scenery52.mmd Diagrams52.mmd Definitions52.mmd Revisions52.mmd -o NGM_Module_Specifications_52.html '

