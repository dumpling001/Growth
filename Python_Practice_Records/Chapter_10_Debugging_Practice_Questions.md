Chapter 10 – Debugging Practice Questions


1. Write an assert statement that triggers an AssertionError if the variable spam is an integer less than 10.

assert spam >= 10, 'The spam variable is less than 10.'

2. Write an assert statement that triggers an AssertionError if the variables eggs and bacon contain strings that are the same as each other, even if their cases are different (that is, 'hello' and 'hello' are considered the same, and 'goodbye' and 'GOODbye' are also considered the same).

assert eggs.lower() != bacon.lower(), 'The eggs and bacon variables contain the same string (case insensitive).'

3. Write an assert statement that always triggers an AssertionError.

assert False, 'Write an assert statement that always triggers an AssertionError.'

or

assert 1 != 1 , 'Write an assert statement that always triggers an AssertionError.'

4. What are the two lines that your program must have in order to be able to call logging.debug()?

import logging
logging.basicConfig(level=logging.DEBUG, format=' %(asctime)s - %(levelname)s - %(message)s')

5. What are the two lines that your program must have in order to have logging.debug() send a logging message to a file named programLog.txt?

import logging
logging.basicConfig(filename='programLog.txt', level=logging.DEBUG, format=' %(asctime)s - %(levelname)s - %(message)s')

6. What are the five logging levels?

DEBUG
INFO
WARNING
ERROR
CRITICAL


7. What line of code can you add to disable all logging messages in your program?

logging.disable(logging.CRITICAL)

8. Why is using logging messages better than using print() to display the same message?

Once we're done debugging, we'll end up spending a lot of time removing print() calls from our code for each log message. We might even accidentally remove some print() calls that were being used for nonlog messages. The nice thing about log messages is that you're free to fill your program with as many as you like, and you can always disable them later by adding a single logging.disable(logging.CRITICAL) call. Unlike print(), the logging module makes it easy to switch between showing and hiding log messages.

9. What are the differences between the Step, Over, and Out buttons in the Debug Control window?

STEP will cause the debugger to execute the next line of code and then pause again. If the next line of code is a function call, the debugger will "step into" that function and jump to the first line of code of that function.

OVER will execute the next line of code, similar to the STEP button. However, if the next line of code is a function call, the OVER button will "step over" the code in the function.

OUT will cause the debugger to execute lines of code at full speed until it returns from the current function.

10. After you click Go in the Debug Control window, when will the debugger stop?

Clicking the GO button will cause the program to execute normally until it terminates or reaches a breakpoint.

11. What is a breakpoint?

A breakpoint can be set on a specific line of code and forces the debugger to pause whenever the program execution reaches that line.

12. How do you set a breakpoint on a line of code in IDLE?

To set a breakpoint, right-click the line in the file editor and select Set Breakpoint.
