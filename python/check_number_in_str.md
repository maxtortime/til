Reference: http://stackoverflow.com/questions/17681655/python-if-a-word-contains-a-digit

```python
if any(ch.isdigit() for ch in word):
    print word, 'contains a digit'
```

Using at this problem, https://www.acmicpc.net/problem/1152
