# enumerate()
Before we go into the definition of enumerate() in Python. Lets define what **__iterator__** is.
An **__iterator__** is defined quite simply as an object representing a stream of data.

[enumerate()](https://docs.python.org/2/library/functions.html#enumerate)

Syntax: `enumerate(sequence, start = 0)`

enumerate() function adds a counter to an iterable.

sequence must be a sequence, an iterator, or some other object which supports iteration.

counter by default starts at 0, you can change that behaviour by passing an integer as the new counter start.

```python
months = ['oct','nov','dec']
list(enumerate(months))
```
```[(0, 'oct'), (1, 'nov'), (2, 'dec')]```

You can also use a for loop to bind the counter and actual element in your iterator to print them separately instead of a tuple as shown above

```python
for count,elem in enumerate(months,start = 10):
  print count, elem
  ```
  
``` 
10 oct

11 nov

12 dec



