https://stackoverflow.com/questions/17958347/how-can-i-convert-a-python-urandom-to-a-string

```python
from base64 import b64encode
from os import urandom

random_bytes = urandom(64)
token = b64encode(random_bytes).decode('utf-8')`

```
