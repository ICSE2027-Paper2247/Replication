Pylsy
=====

[![Build Status](https://travis-ci.org/Leviathan1995/Pylsy.svg?branch=master)](https://travis-ci.org/Leviathan1995/Pylsy)
[![PyPI version](https://badge.fury.io/py/Pylsy.svg)](https://badge.fury.io/py/Pylsy)

Pylsy is a simple Python library for drawing tables in the terminal/console. Just two lines of code! 

![Screenshot](https://raw.githubusercontent.com/Leviathan1995/Pylsy/master/pzi/span.png)
 
Install
-------

    pip3 install pylsy

Sample Usage
------------

```python
from pylsy import pylsytable

# Create a table with column headers
table = pylsytable(["name", "origin", "level", "status"])

# Add data by column
table.add_data("name", ["luna", "小明", "café"])
table.add_data("origin", ["\U0001F1EF\U0001F1F5", "\U0001F1E8\U0001F1F3", "\U0001F1EB\U0001F1F7"])
table.add_data("level", [42, 108, 7])

# Append more rows
table.append_data("name", "leviathan")
table.append_data("origin", "\U0001F30A")
table.append_data("level", 99)

# ANSI colors work too
table.append_data("status", "\x1b[32mactive\x1b[0m")
table.append_data("status", "\x1b[33midle\x1b[0m")
table.append_data("status", "\x1b[31maway\x1b[0m")
table.append_data("status", "\x1b[36monline\x1b[0m")

print(table)
```

License
-------
MIT
