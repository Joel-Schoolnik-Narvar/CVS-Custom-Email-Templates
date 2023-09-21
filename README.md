# CVS-Custom-Email-Templates

These are the legacy email templates.  As of 2023, CVS has not migrated to WYSIWYG because of the highly convoluted logic in their live templates with would require testing resources for the migration that CVS does not have.  

## How to Fork and Merge


## How the Templates Work
At a high level, the templates are comipiled from blocks of HTML.  The HTML exists as string values within the json file which is an email template.  The hlocks are organized by and value called "html" - which is an html file (saved as a string) that references the blocks.  

A best practice for scalability would be to make many blocks for different conditions and show or hide them based on flags in data from the Order API.  However, as the templates were iterated on over time, the logic was added haphazardly to the individual blocks.  Therefore and addition requires careful dissection of the relevant blocks to add to the new logic.  Reccomendation going forward is to simply create new blocks.  

