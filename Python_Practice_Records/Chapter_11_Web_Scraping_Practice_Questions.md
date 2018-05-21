Chapter 11 Web Scraping Practice Questions



1. Briefly describe the differences between the webbrowser, requests, BeautifulSoup, and selenium modules.

webbrowser: Comes with Python and opens a browser to a specific page.
Requests: Downloads files and web pages from the Internet.
BeautifulSoup: Parses HTML, the format that web pages are written in.
Selenium: Launches and controls a web browser. Selenium is able to fill in forms and simulate mouse clicks in this browser.

2. What type of object is returned by requests.get()? How can you access the downloaded content as a string value?

The type of object that returned by requests.get() is a Response object.

```python
import requests
res = requests.get('https://painset.com')
type(res)
```
This will get result: <class 'requests.models.Response'>.

If the request succeeded, the downloaded web page is stored as a string in the Response object's text variable. Such as:

res.text


3. What Requests method checks that the download worked?

A ways to check for success is to call the raise_for_status() method on the Response object. Such as:

res.raise_for_status()

4. How can you get the HTTP status code of a Requests response?

By res.status_code. if it is equal to the value of requests.codes.ok, then everything went fine.

5. How do you save a Requests response to a file?

To write the web page to a file, you can use a for loop with the Response object's iter_content() method.

```python
import requests
res = requests.get('https://.../...txt')
res.raise_for_status()
playFile = open('RomeoAndJuliet.txt', 'wb')
for chunk in res.iter_content(100000):
  playFile.write(chunk)
playFile.close()
```

6. What is the keyboard shortcut for opening a browser’s developer tools?

Chrome and IE:
Command + Option + I in OS X,
or F12 for Windows.

7. How can you view (in the developer tools) the HTML of a specific element on a web page?

Right-click the specific element on the page and select Inspect Element from the context menu that appears.

8. What is the CSS selector string that would find the element with an id attribute of main?

'#main'

9. What is the CSS selector string that would find the elements with a CSS class of highlight?

'.highlight'

10. What is the CSS selector string that would find all the <div> elements inside another <div> element?

'div div'

11. What is the CSS selector string that would find the <button> element with a value attribute set to favorite?

'button[value="favorite"]'

12. Say you have a Beautiful Soup Tag object stored in the variable spam for the element <div>Hello world!</div>. How could you get a string 'Hello world!' from the Tag object?

spam.getText()

13. How would you store all the attributes of a Beautiful Soup Tag object in a variable named linkElem?

linkElem.attrs

14. Running import selenium doesn’t work. How do you properly import the selenium module?

from selenium import webdriver

15. What’s the difference between the find_element_* and find_elements_* methods?

The find_element_* methods return a single WebElement object, representing the first element on the page that matches your query.

The find_elements_* methods return a list of WebElement \_\* objects for every matching element on the page.

16. What methods do Selenium’s WebElement objects have for simulating mouse clicks and keyboard keys?

click() method and send_keys()

17. You could call send_keys(Keys.ENTER) on the Submit button’s WebElement object, but what is an easier way to submit a form with Selenium?

Calling the submit() method on any element will have the same result as clicking the Submit button for the form that element is in.

18. How can you simulate clicking a browser’s Forward, Back, and Refresh buttons with Selenium?

browser.forward()
browser.back()
browser.refresh()
