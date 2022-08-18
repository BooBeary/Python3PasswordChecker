# PYTHON PASSWORD LEAK CHECKER

#### By: Boo

## Description

'''

This program takes a password input in the terminal arguments, uses hashlib to create a hexidecimal hash of the password, request the data of the first five characters of the hash from [haveibeenpwned](https://haveibeenpwned.com/), compares the recieved data against the number of leaks recorded for a matching password, and displays the number of leaks in terminal.

'''

## HOW TO USE THIS PROGRAM

'''

Run **main.py** with python3, for the arguments input the password you want to check, use either an escape sequence before every special character in your terminal for example:

> ``~python3 main.py P4\$\$w0rD5aMp\!3``

or you can put the password in double quotes:

> ``~python3 main.py "P4$$w0rD5aMp!3"``

'''

The terminal will display a message depending on the number of leaks recorded:

> ``~python3 main.py "P4$$w0rD5aMp!3"``
> 
> P4$$w0rD5aMp!3 was found *LEAKS RECORDED* times, you should probably change your password.

or in the case that no matching hashes were found:

> ``~python3 main.py "P4$$w0rD5aMp!3"``
> 
> P4$$w0rD5aMp!3 was NOT found. Nice ; )

the program then returns to terminal after printing:

> All done, returning to terminal.

'''

## EXAMPLE

'''

> ``~python3 main.py "P4$$w0rD5aMp!3"``
> 
> P4$$w0rD5aMp!3 was NOT found. Nice ; )
> 
> All done, returning to terminal.
> 
> ``~|``

'''
