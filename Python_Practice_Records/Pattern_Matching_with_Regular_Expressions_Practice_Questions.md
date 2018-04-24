Practice Questions

Q1. What is the function that creates Regex objects?

import re
phoneNumRegex = re.compile(r'\d\d\d-\d\d\d\d-\d\d\d')

Q2. Why are raw strings often used when creating Regex objects?

Since regular expressions frequently use backslashes in them, it is convenient to pass raw strings to the re.compile() function instead of typing extra backslashes.

Q3. What does the search() method return?

The search() method will return None if the regex pattern is not found in the string. If the pattern is found, the search() method returns a match object.

Q4. How do you get the actual strings that match the pattern from a Match object?

If a match object is not the null value None, we can call grou() on the match object to return the match result.

Q5. In the regex created from r'(\d\d\d)-(\d\d\d-\d\d\d\d)', what does group 0 cover? Group 1? Group 2?

Group 0: (\d\d\d)-(\d\d\d-\d\d\d\d)
Group 1: (\d\d\d)
Group 2: (\d\d\d-\d\d\d\d)
