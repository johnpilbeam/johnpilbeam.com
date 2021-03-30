---
layout: post
title:  "Messy Data"
date:   2021-03-10 10:20:00 +0000
categories: data update
---
In libraries there is often a lot of raw data collected by systems and vendors. This data has the potential to provide insights for improving library services. However, the data is often incomplete with missing cells, and entries can be inconsistent (e.g. "Math, Maths, Mathematics,"). Here are some free or readily available tools that help with data clean up.

## Microsoft Excel
As a Mac user it doesn't feel great to recommend that you use Microsoft Excel on Windows, but the sad truth is that the Windows version has some powerful features that are missing from the Mac version.

### Fixing missing data
If you have a spreadsheet with some columns completed, but others incomplete, you might still be able to use a [shortcut to add the missing data](https://exceljet.net/lessons/shortcut-recipe-fill-in-missing-data). For example you might have a spreadsheet logging user access to a system, where every row has a user's email address in column E, but user's department is missing from column H. If the user's email includes their department name (e.g alice.bob@bunnystudies.uni.edu), then we're in luck and we can use a shortcut:

- Select everthing in the current worksheet with <code>Ctrl + A</code>.
- Use <code>Ctrl + A</code> (Go To Special) select only the blank cells.
- Enter a formula that simply gets the value from cell E(row number) e.g. <code>=E2</code>.


### Convert a Formula to Value in Excel
Once you have the missing data filled in, you will need to [convert the text created by the formula into static text](https://excelchamps.com/blog/convert-to-value/) so it can be edited:
- Select the range of the cells where you have formulas.
- Press <code>Ctrl + C</code> to copy the cells.
- Press <code>Alt + E S V</code>.

### Replace static email addresses with department names
Select the column with the email addresses to replace with department names. Then use Replace (Edit > Find > Replace) to replace each group of emails with their department name e.g. find <code>*@bunnystudies.uni.edu</code> and replace with <code>Bunny Studies</code>.

### Analyse data
The Analyse Data feature in Excel (Windows only 🙁️) is incredible for quickly creating PivotTables through natural language queries. This [Microsoft guide](https://support.microsoft.com/en-gb/office/analyze-data-in-excel-3223aab8-f543-4fda-85ed-76bb0295ffc4?ui=en-us&rs=en-gb&ad=gb) explains the capabilities very well.

## OpenRefine
If you are working with messy messy data in libraries, I would highly recommend the [Library Carpentry lesson on OpenRefine](https://librarycarpentry.org/lc-open-refine/). OpenRefine is a "free, open source, powerful tool for working with messy data". The [Faceting and filtering](https://librarycarpentry.org/lc-open-refine/04-faceting-and-filtering/index.html) features of OpenRefine are some of the most useful. Text facets can be used to fix inconsistencies and spelling mistakes made during the original data entry or capture process.
