Chapter 12 Working with Excel Spreadsheets Practice Questions



1. What does the openpyxl.load_workbook() function return?

The openpyxl.load_workbook() function takes in the filename and returns a value of the workbook data type. This Workbook object represents the Excel file, a bit like how a File object represents an opened text file.

2. What does the get_sheet_names() workbook method return?

A list of all the sheet names in the workbook.

3. How would you retrieve the Worksheet object for a sheet named 'Sheet1'?

sheet = wb[Sheet1]

4. How would you retrieve the Worksheet object for the workbook’s active sheet?

sheet = wb.active

5. How would you retrieve the value in the cell C5?

sheet['C5'].value
sheet['C5'].value

6. How would you set the value in the cell C5 to "Hello"?

sheet['C5'] = 'Hello'

7. How would you retrieve the cell’s row and column as integers?

cell.row
column_index_from_string('A')

8. What do the max_column and max_row sheet methods return, and what is the data type of these return values?

max_column() returns an integer rather than the letter that appears in Excel. max_row is the same.

9. If you needed to get the integer index for column 'M', what function would you need to call?

column_index_from_string('M')

10. If you needed to get the string name for column 14, what function would you need to call?

get_column_letter(14)

11. How can you retrieve a tuple of all the Cell objects from A1 to F1?

tuple(sheet['A1':'F1'])

12. How would you save the workbook to the filename example.xlsx?

wb.save('example.xlsx')

13. How do you set a formula in a cell?

sheet['A10'] = '=SUM(A1:A9)'

15. How would you set the height of row 5 to 100?

sheet.row_dimensions[5].height = 100

16. How would you hide column C?

sheet.column_dimensions['C'].width = 0

17. Name a few features that OpenPyXL 2.3.3 does not load from a spreadsheet file.

Load charts.

18. What is a freeze pane?

For spreadsheet too large to be displayed all at once, it's helpful to "freeze" a few of the top rows or leftmost columns onscreen. Frozen column or row headers, for example, are always visible to the user even as they scroll through the spreadsheet. These are known as freeze panes.

19. What five functions and methods do you have to call to create a bar chart?

The following five functions and methods we have to call to create a bar chart:

openpyxl.chart.Reference()
openpyxl.chart.Series()
openpyxl.chart.BarChart()
chartObj.append(seriesObj)
sheet.add_chart()


Step1: Create a Reference object from a rectangular selection of cells. e.g.

refObj = openpyxl.chart.Reference(sheet, min_col=1, min_row=1, max_col=1, max_row=10)

Step2: Create a Series object by passing in the Reference object. e.g.

seriesObj = openpyxl.chart.Series(refObj, title='First series')

Step3: Create a Chart object. e.g.

chartObj = openpyxl.chart.BarChart()

Step4: Append the Series object to the Chart object. e.g.

chartObj.append(seriesObj)

Step5: Add the Chart object to the Worksheet object, optionally specifying which cell the top left corner of the chart should be positioned. e.g.

sheet.add_chart(chartObj, 'C5')
