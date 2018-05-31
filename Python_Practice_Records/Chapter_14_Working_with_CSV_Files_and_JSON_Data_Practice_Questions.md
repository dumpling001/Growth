Chapter 14 – Working with CSV Files and JSON Data

Practice Questions

1. What are some features Excel spreadsheets have that CSV spreadsheets don’t?

CSV files are simple, lacking many of the features of an Excel spreadsheet. For example, CSV Files

* Don't have types for their values-everything is a string
* Don't have settings for font size or color
* Don't have multiple worksheets
* Can't specify cell widths and heights
* Can't have merged Cells
* Can't have images or charts embedded in them.

2. What do you pass to csv.reader() and csv.writer() to create Reader and Writer objects?

To read a CSV file with the csv module, first open it using the open() function, just as you would any other text file. Pass the File object that open() returns to the csv.reader() function. This will return a Reader object for you to use.

A Writer object lets you write data to a CSV file. To create a Writer object, you use the csv.writer() function.

3. What modes do File objects for reader and Writer objects need to be opened in?

'w' mode.

4. What method takes a list argument and writes it to a CSV file?

writerow() method.

5. What do the delimiter and lineterminator keyword arguments do?

The delimiter is the character that appears between cells on a row.

The line terminator is a newline. you change characters to different values by using the delimiter and lineterminator keyword arguments with csv.writer().

6. What function takes a string of JSON data and returns a Python data structure?

json.loads()

7. What function takes a Python data structure and returns a string of JSON data?

json.dumps()
