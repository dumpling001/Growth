20180402

What's the best way to start learning django? [closed]
https://stackoverflow.com/questions/4048973/whats-the-best-way-to-start-learning-django

https://docs.djangoproject.com/en/2.0/intro/tutorial01/

How do I get started with web development using Django?
https://www.quora.com/How-do-I-get-started-with-web-development-using-Django

The Django Book
http://djangobook.py3k.cn/2.0/

How to solve ReadTimeoutError: HTTPSConnectionPool(host='pypi.python.org', port=443) with pip?
https://stackoverflow.com/questions/43298872/how-to-solve-readtimeouterror-httpsconnectionpoolhost-pypi-python-org-port


2018.4.3 7:46

~ ⮀ pip install django
Collecting django
 Using cached Django-1.11.11-py2.py3-none-any.whl
Requirement already satisfied: pytz in /System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python (from django) (2013.7)
matplotlib 1.3.1 requires nose, which is not installed.
matplotlib 1.3.1 requires tornado, which is not installed.
prompt-toolkit 1.0.15 has requirement six>=1.9.0, but you'll have six 1.4.1 which is incompatible.
Installing collected packages: django

~ ⮀ **sudo pip install django**
The directory '/Users/###/Library/Caches/pip/http' or its parent directory is not owned by the current user and the cache has been disabled. Please check the permissions and owner of that directory. If executing pip with sudo, you may want sudo's -H flag.
The directory '/Users/###/Library/Caches/pip' or its parent directory is not owned by the current user and caching wheels has been disabled. check the permissions and owner of that directory. If executing pip with sudo, you may want sudo's -H flag.
Collecting django
 Downloading Django-1.11.11-py2.py3-none-any.whl (6.9MB)
   100% |████████████████████████████████| 7.0MB 28kB/s
Requirement already satisfied: pytz in /System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python (from django) (2013.7)
matplotlib 1.3.1 requires nose, which is not installed.
matplotlib 1.3.1 requires tornado, which is not installed.
prompt-toolkit 1.0.15 has requirement six>=1.9.0, but you'll have six 1.4.1 which is incompatible.
Installing collected packages: django
Successfully installed django-1.11.11


~/PYTHON ⮀ sudo pip install --user tornado
The directory '/Users/###/Library/Caches/pip/http' or its parent directory is not owned by the current user and the cache has been disabled. Please check the permissions and owner of that directory. If executing pip with sudo, you may want sudo's -H flag.
The directory '/Users/###/Library/Caches/pip' or its parent directory is not owned by the current user and caching wheels has been disabled. check the permissions and owner of that directory. If executing pip with sudo, you may want sudo's -H flag.
Collecting tornado
 Downloading tornado-5.0.1.tar.gz (504kB)
   100% |████████████████████████████████| 512kB 490kB/s
Collecting futures (from tornado)
 Downloading futures-3.2.0-py2-none-any.whl
Collecting singledispatch (from tornado)
 Downloading singledispatch-3.4.0.3-py2.py3-none-any.whl
Collecting backports_abc>=0.4 (from tornado)
 Downloading backports_abc-0.5-py2.py3-none-any.whl
Requirement already satisfied: six in /System/Library/Frameworks/Python.framework/Versions/2.7/Extras/lib/python (from singledispatch->tornado) (1.4.1)
prompt-toolkit 1.0.15 has requirement six>=1.9.0, but you'll have six 1.4.1 which is incompatible.
Installing collected packages: futures, singledispatch, backports-abc, tornado
 Running setup.py install for tornado ... done
Successfully installed backports-abc-0.5 futures-3.2.0 singledispatch-3.4.0.3 tornado-5.0.1
~/PYTHON ⮀ sudo pip install --user nose
The directory '/Users/###/Library/Caches/pip/http' or its parent directory is not owned by the current user and the cache has been disabled. Please check the permissions and owner of that directory. If executing pip with sudo, you may want sudo's -H flag.
The directory '/Users/###/Library/Caches/pip' or its parent directory is not owned by the current user and caching wheels has been disabled. check the permissions and owner of that directory. If executing pip with sudo, you may want sudo's -H flag.
Requirement already satisfied: nose in /Library/Python/2.7/site-packages (1.3.7)
prompt-toolkit 1.0.15 has requirement six>=1.9.0, but you'll have six 1.4.1 which is incompatible.
~/PYTHON ⮀ sudo pip install --user prompt-toolkit
The directory '/Users/###/Library/Caches/pip/http' or its parent directory is not owned by the current user and the cache has been disabled. Please check the permissions and owner of that directory. If executing pip with sudo, you may want sudo's -H flag.
The directory '/Users/###/Library/Caches/pip' or its parent directory is not owned by the current user and caching wheels has been disabled. check the permissions and owner of that directory. If executing pip with sudo, you may want sudo's -H flag.
Requirement already satisfied: prompt-toolkit in /Library/Python/2.7/site-packages (1.0.15)
Requirement already satisfied: wcwidth in /Library/Python/2.7/site-packages (from prompt-toolkit) (0.1.7)
Collecting six>=1.9.0 (from prompt-toolkit)
 Downloading six-1.11.0-py2.py3-none-any.whl
Installing collected packages: six
Successfully installed six-1.11.0
~/PYTHON ⮀ sudo pip install --user tornado
The directory '/Users/###/Library/Caches/pip/http' or its parent directory is not owned by the current user and the cache has been disabled. Please check the permissions and owner of that directory. If executing pip with sudo, you may want sudo's -H flag.
The directory '/Users/###/Library/Caches/pip' or its parent directory is not owned by the current user and caching wheels has been disabled. check the permissions and owner of that directory. If executing pip with sudo, you may want sudo's -H flag.
Requirement already satisfied: tornado in /Users/###/Library/Python/2.7/lib/python/site-packages (5.0.1)
Requirement already satisfied: futures in /Users/###/Library/Python/2.7/lib/python/site-packages (from tornado) (3.2.0)
Requirement already satisfied: singledispatch in /Users/###/Library/Python/2.7/lib/python/site-packages (from tornado) (3.4.0.3)
Requirement already satisfied: backports_abc>=0.4 in /Users/###/Library/Python/2.7/lib/python/site-packages (from tornado) (0.5)
Requirement already satisfied: six in /Users/###/Library/Python/2.7/lib/python/site-packa


20180403 21:32

http://initd.org/psycopg/tarballs/PSYCOPG-2-7/
Download psycopg2-2.7.1.tar.gz

Position: /Users/###/Downloads


https://www.postgresql.org/download/macosx/
Download PostgreSQL installer, 2hours - not finished


https://stackoverflow.com/questions/35313876/after-installing-with-pip-jupyter-command-not-found

pip install jupyter
or
export PATH=~/anaconda2/bin:$PATH


20180404 7:07
Download PostgreSQL installer finished, 138MB
Install PostgresSQL finished.

Start a project:
mkdir django
django-admin.py startproject mysite


20180405 20:31

mysite/
    \__init__.py
    manage.py
    settings.py
    urls.py
->> python manage.py help

Type 'manage.py help <subcommand>' for help on a specific subcommand.

->> python manage.py runserver
open http://127.0.0.1:8000/

如果想和其他开发人员共享同一开发站点的话，需要做另外一些设置。

The Django Book 第二章:入门 结束。

20180406 21:08

创建了第一个Django的web页面。很有成就感。

20180408 8:28

实现了一个动态页面。

觉得下次应该把代码传到Github上去。这样可以直观地看代码上的变化和进度。

2018-4-9 20:45
Create repository in Github. And commit local code to the repository.

Begin to learn chapter 4: Django Templates.
need to use python manage.py shell in these examples, or Django will throw an exception.

Next: Creating Template Objects

2018.4.10

Next: Dictionaries and Contexts

2018.4.11 19:59-20:37
Dictionaries and Contexts:

Those are the fundamentals of using the Django template system: just write a template string, create a Template object, create a Context, and call the render() method.

Next: Context Variable Lookup

20180412 20:01

Next:
Chapter 3: Django Templates - Basic Template Tags and Filters

20180413 8:12

NEXT: For example, if your context contains a list of (x,y) coordinates called points, you could use the following to output the list of points:

20180413 20:49
Stop to learn Django now. Keep focus on automatetheboringstuff.

Finished 95%:
https://automatetheboringstuff.com/chapter4/

20180417 20:50
Finished 95%:
https://automatetheboringstuff.com/chapter6/
Chapter 6 – Manipulating Strings

20180418 30min
Chapter 7 – Pattern Matching with Regular Expressions
https://automatetheboringstuff.com/chapter7/
Next
Optional Matching with the Question Mark

20180420 30min

Next
Matching Newlines with the Dot Character

20180421 30min

NEXT:
Project: Phone Number and Email Address Extractor

20180423 30min
NEXT:
Practice Questions

20180503 10min
https://automatetheboringstuff.com/chapter8/
NEXT:
Project: Generating Random Quiz Files

20180506 4-5 hours

Chapter 9 – Organizing Files finished.

20180508 40mins
https://automatetheboringstuff.com/chapter10/

NEXT: Assertions


20180515 1 hour

Issue:
ImportError: No module named pyperclip

Try1:(No use)
https://stackoverflow.com/questions/3819449/how-to-uninstall-python-2-7-on-a-mac-os-x-10-6-4
Remove the symbolic links in /usr/local/bin that point to this Python version see ls -l /usr/local/bin | grep '../Library/Frameworks/Python.framework/Versions/2.7' and then run the following command to remove all the links:

cd /usr/local/bin/
ls -l /usr/local/bin | grep '../Library/Frameworks/Python.framework/Versions/2.7' | awk '{print $9}' | tr -d @ | xargs rm
I

Try2(Real solution):

Install python3
Step1: Download
https://www.python.org/downloads/release/python-365/

Step2: Install

Step3: pip3 install --upgrade pip

Step4: python3 -m pip install pyperclip

Rerun, succeeded.

NEXT:

https://automatetheboringstuff.com/chapter11/

Downloading a Web Page with the requests.get() Function

20180516:

NEXT:
Saving Downloaded Files to the Hard Drive

In Chrome and Internet Explorer for Windows, the developer tools are already installed, and you can press F12 to make them appear. Pressing F12 again will make the developer tools disappear. In Chrome, you can also bring up th developer tools by selecting View->Developer->Developer Tools. In OS X, pressing Command -OPTION-I will open Chrome's Developer Tools.

import os
os.getcwd()
os.chdir('/Users/xxx/Applications')

Correct:
exampleSoup = bs4.BeautifulSoup(exampleFile, "html.parser")

Incorrect:
exampleSoup = bs4.BeautifulSoup(exampleFile)

NEXT:
Finding an Element with the select() Method

20180517:

I encounter a issue this morning:

len(elems) is 0, I tried many ways but failed. Tonight I checked example.html, and found it was blan, which is very strange. I copy the content to it, then run commands, it works. I wonder why I didn't use this way this morning and waste my precious 15 minutes.

Path is important.
```python
#! /usr/bin/env python3
```
chmod +x lucky.py

./lucky.py how to get a high paid job

20180519:

NEXT:
Controlling the Browser with the selenium Module

20180520

Issue1:
Q: How to find file path in OS X?
A: Option + Space
-> "Show all in Finder" at the bottom of the poped-up window
-> select the target file -> right-click, select "Get Info"
-> Copy the Where info
-> Done.

Issue 2:
Q: How to use chromedriver in python3?
A:
```python
>>> from selenium import webdriver
>>> driver_path = "/usr/local/bin/chromedriver"
>>> driver = webdriver.Chrome(driver_path)
```

Issue 3: zsh: bad assignment

Solution:
Removed the extra white spaces before and after the = and it worked.

Help post:
Installing ChromeDriver on macOS & System PATH Setup
https://www.kenst.com/2015/03/installing-chromedriver-on-mac-osx/

New way to install ChromeDriver:
brew tap caskroom/cask
brew cask install chromedriver

Issue 4: Error: It seems there is already a Binary at '/usr/local/bin/chromedriver'; not linking.

Solution:
rm -rf /usr/local/bin/chromedriver

The selenium part didn't finish very good because encountering many issues, one of which is environment variable setting.

Feel depressed. Anyway, will move to the next chapter.

20180521

https://automatetheboringstuff.com/chapter12/

Chapter 12 – Working with Excel Spreadsheets

pip3 install openpyxl==2.1.4
pip3 install --upgrade openpyxl

import os
os.getcwd()
os.chdir(path)

NEXT:

Converting Between Column Letters and Numbers

20180522:

NEXT:
Ideas for Similar Programs (The first one.)

Issue: ModuleNotFoundError: No module named 'census2010'

Unresolved.

Issue: DeprecationWarning: Call to deprecated function get_sheet_by_name (Use wb[sheetname]).

Solution: Use: sheet = wb["UseThisSheet"] instead.


20180523:

```python
>>> wb.get_sheet_names()

Warning (from warnings module):
  File "/Users/liuhuajiao/readCensusExcel.py", line 1
    #! python3
DeprecationWarning: Call to deprecated function get_sheet_names (Use wb.sheetnames).
['Sheet']
>>> wb.sheetnames
['Sheet']
```

DeprecationWarning: Call to deprecated function remove_sheet (Use wb.remove(worksheet) or del wb[sheetname]).

NEXT: Writing Values to Cells

NEXT: Ideas for Similar Programs (The second one.)

20180524:

NEXT: Font Objects

NEXT: Practice Questions

20180527

Chapter 14 – Working with CSV Files and JSON Data

NEXT: Writer Objects
