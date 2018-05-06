# Chapter 9 – Organizing Files
# Practice Questions

1. What is the difference between shutil.copy() and shutil.copytree()?

shutil.copy() will copy a single file.

shutil.copytree() will copy an entire folder and every folder and file contained in it. Calling shutil.copytree(source, destination) will copy the folder at the path source, along with all of its files and subfolders, to the folder at the path destination. The source and destination parameters are both strings. The function returns a string of the path of the copied folder.

2. What function is used to rename files?

shutil.move will rename files.

3. What is the difference between the delete functions in the send2trash and shutil modules?

shutil.rmtree() function irreversibly deletes files and folders.

send2trash will send folders and files to computer's trash or recycle bin instead of permanently deleting them.

4. ZipFile objects have a close() method just like File objects’ close() method. What ZipFile method is equivalent to File objects’ open() method?

ZipFile method is equivalant to File objects' open() method. For example,

```python
import zipfile
newZip = zipfile.ZipFile('new.zip', 'w')
```

Source: https://automatetheboringstuff.com/chapter9/
