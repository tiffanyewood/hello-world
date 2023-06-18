Sets are unordered collections of UNIQUE elements - no repeating objects


```python
myset=set()
```


```python
myset.add(1)
```


```python
myset
```




    {1}




```python
myset.add(2)
```


```python
myset
```




    {1, 2}




```python
myset.add(2)
```


```python
myset
```




    {1, 2}



^See above, can't add value twice because they must be unique


```python
myset.add("two")
```


```python
myset
```




    {1, 2, 'two'}




```python
myset.add("TWO","Two")
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[11], line 1
    ----> 1 myset.add("TWO","Two")


    TypeError: set.add() takes exactly one argument (2 given)


^.add only allows to add 1 argument to a set at a time


```python
myset.add("TWO")
```


```python
myset.add("Two")
```


```python
myset.add("2")
```


```python
myset
```




    {1, 2, '2', 'TWO', 'Two', 'two'}



^ variations of the number 2 can be added because they are all unique


```python
mylist=[1,1,1,1,1,1,2,2,2,2,2,3,3,3,3,3,3,3,]
```


```python
set(mylist)
```




    {1, 2, 3}




```python

```


```python

```


```python

```


```python

```
