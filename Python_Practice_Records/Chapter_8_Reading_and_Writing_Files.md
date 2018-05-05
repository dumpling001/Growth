#Chapter 8 – Reading and Writing Files

Practice Questions



1. What is a relative path relative to?

A relative path is relative to the program's current working directory.

2. What does an absolute path start with?

An absolute path always begins with the root folder.

3. What do the os.getcwd() and os.chdir() functions do?

os.getcwd() get the current working directory as a string value.

os.chdir() change the current working directory to the argument.

4. What are the . and .. folders?

A single period (.) for a folder name is shorthand for "this directory." Two periods (..) means "the parent folder."

5. In C:\\bacon\\eggs\\spam.txt, which part is the dir name, and which part is the base name?

Dir name is C:/\bacon/\eggs/, base name is spam.txt.

6. What are the three “mode” arguments that can be passed to the open() function?

Read mode: open('test.txt', 'r'),
Write mode: open('test.txt', 'w'),
Append mode: open('test.txt', 'a').

7. What happens if an existing file is opened in write mode?

It will overwrite the existing file and start from scratch, just like when you overwrite a variable's value with a new value.

8. What is the difference between the read() and readlines() methods?

read() method returns the contents of a file as a single large string value.

readline() method get a list of string values from the file, one string for each line of text.

9. What data structure does a shelf value resemble?

A shelf value resemble dictionary data structure.
