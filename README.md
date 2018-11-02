# Syllabify.py

syllabify.py is a Python module for syllabifying ARPABET transcriptions; 
the method used is informed by subtle details of English phonology.

* See `manual.pdf` for usage

# Why fork the original package?

The only two reason I'm forking this project are:

 + The original package uses `xrange` which is not compatible with Python 3.
 + The original package could not be installed via `pip`.
 
Since I wanted both of those things in a project I found myself working on one day, I thought I'd fork the original project.

# Installing

You can install this project via `pip` with:

```bash
pip install git+https://github.com/formigone/syllabify.git
```

# Example

```python
from formigone.syllabify import syllabify

arpa = ['L', 'ER1', 'N', 'IH0', 'NG']
syllabify(arpa, flatten=True)
# => [
#   ['L', 'ER1'],
#   ['N', 'IH0', 'NG']
# ]
```
