# csv-protect-columns

This tool helps you protect CSV column data from incorrect manipulation when opening in MS Excel.

## Why

A friend of mine uses webshop software and allows export and import of product data. He uses the 
export and import to make bulk adjustments of price and other description edits. The issue was that 
when opening in Excel his product codes (which often start with zero) had been interpreted by Excel 
as numbers, and therefore leading zeros had been lost.

I wrote this little tool to help him.

## How to use
      
1. Choose Protect CSV
1. Drag/Drop or Browse for the original CSV file
1. Select the columns to protect
1. Click the download button
1. Edit the downloaded CSV in Excel
1. Return to this page, choose Unprotect CSV
1. Drag/Drop or Browse for the editted CSV file
1. The Unprotected CSV will download automatically
1. Voila!
      
## How it works
      
When protecting a CSV the code adds two vertical bars (like "||") to the front of the value in protected columns to ensure that Excel treats the column as text, and leaves it alone!

When unprotecting a CSV the code removes all groups of double vertical bars it finds at the beginning of any column value.

## Disclaimer

I take no responsibility for your data. Please use this tool with care and attention.

## Another disclaimer

I am a developer but I am not really a front-end developer. This project has been cobbled together 
from bits of the internet, and while the outcome is suitable, the underlying code could do with
some love.
