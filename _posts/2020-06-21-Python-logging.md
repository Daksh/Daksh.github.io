---
layout: post
title: How to use the `logging` python module
order: 3
---

I had been always `print`ing all my output and the debugging statements as well. I had to run a script as `python3 script.py > out.txt 2>err.txt`.

It was getting a little difficult to understand when what is happening and this seemed to hacky. So I started looking at alternatives and came across a built-in python library called `logging`.

After going through a few different resource and StackOverflow answers, I came up with the following short script which works perfectly in my use case. Feel free to adjust the date-format/log-format as per your preference.

```python
import logging

logging.basicConfig(
    filename='script.log',
    filemode='w', #can do 'a' for append
    level=logging.DEBUG,
    format="%(asctime)s | %(levelname)s : %(message)s",
    datefmt="%d-%m-%Y %H:%M:%S ",
)

logging.debug("debug message")
logging.info("info message")
logging.warning("warn message")
logging.error("error message")
logging.critical("critical message")
```

## References
1. https://www.geeksforgeeks.org/logging-in-python/
2. https://stackoverflow.com/a/6386990/2806163
3. https://docs.python.org/3.1/library/logging.html
4. https://stackoverflow.com/a/23874319/2806163