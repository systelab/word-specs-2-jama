This script uploads traditional specifications documents from an exported Microsoft Word document to Jama.

# What it does
* Recreates same hierarchy as defined in Microsoft Word
* Uploads texts and specifications
* Uploads images and tables
* Generates a correspondence table between Microsoft Word ids and new Jama ids

# How to use it
1. Export word document as "Web Page, Filtered" with name specs.htm and save it in the save folder location as this script.
1. Open document with Notepad++ and convert to utf8
1. Open index.htm with a browser that has CORS disabled or copy all files to the JAMA server
1. In case using it locally, add localhost to the allowed sites in Jama server using curl
1. Open index.htm and set input data.
1. Review parsed version and, in case everything is correct, upload

# Limitations
* Specifications are defined with following format: SPECKEY[...]:
* Specifications document is an exported htm normally coming from Microsoft Word as "Web Page, Filtered"
* Word sections are defined with headings h1,h2,h3,h4,h5,h6. Any subsection that goes deeper will not work 
