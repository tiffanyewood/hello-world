Tuples are similar to lists BUT they are immutable - once an object is inside a tuple it cannot be reassigned. Tuples also use () instead of [].


```python
t=(1,2,3)
```


```python
mylist=[1,2,3]
```


```python
type(t)
```




    tuple




```python
type(mylist)
```




    list




```python
len(t)
```




    3




```python
t=("one",2)
```


```python
t[0]
```




    'one'




```python
t[-1]
```




    2




```python
t=("a","a","b")
```


```python
t.count("a")
```




    2




```python
t.index("a")
```




    0




```python
t.index("b")
```




    2




```python
t.count("b")
```




    1




```python
t
```




    ('a', 'a', 'b')




```python
mylist[0]="NEW"
```


```python
mylist
```




    ['NEW', 2, 3]




```python
t[0]="NEW"
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[18], line 1
    ----> 1 t[0]="NEW"


    TypeError: 'tuple' object does not support item assignment


^Tuples are immutable, unlike lists. This is good for data integrity because you can't accidentally reassign anything

Only 2 methods are available with tuples: count and index


```python

```
