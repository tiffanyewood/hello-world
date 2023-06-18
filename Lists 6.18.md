```python
my_list=[1,2,3]
```


```python
my_list
```




    [1, 2, 3]




```python
my_list=["STRING",100,23.2]
```


```python
my_list
```




    ['STRING', 100, 23.2]




```python
len(my_list)
```




    3




```python
my_list=["one","two","three"]
```


```python
my_list[0]
```




    'one'




```python
my_list[1:]
```




    ['two', 'three']




```python
your_list=["four","five"]
```


```python
my_list+your_list
```




    ['one', 'two', 'three', 'four', 'five']




```python
our_lists=my_list+your_list
```


```python
our_lists
```




    ['one', 'two', 'three', 'four', 'five']




```python
our_lists[0]="ONE"
```


```python
our_lists
```




    ['ONE', 'two', 'three', 'four', 'five']




```python
our_lists[2].upper()
```




    'THREE'




```python
our_lists
```




    ['ONE', 'two', 'three', 'four', 'five']




```python
our_lists.append("six")
```


```python
our_lists.append("seven")
```


    ---------------------------------------------------------------------------

    AttributeError                            Traceback (most recent call last)

    Cell In[45], line 1
    ----> 1 our_lists.append("seven")


    AttributeError: 'tuple' object has no attribute 'append'



```python
our_lists='ONE', 'two', 'three', 'four', 'five', 'six'
```


```python
our_lists=['one', 'two', 'three', 'four', 'five','six','seven']

```


```python
our_lists
```




    ['one', 'two', 'three', 'four', 'five', 'six', 'seven']




```python
our_lists.pop()
```




    'seven'




```python
our_lists
```




    ['one', 'two', 'three', 'four', 'five', 'six']




```python
popped_item=our_lists.pop()
```


```python
popped_item
```




    'six'




```python
our_lists
```




    ['one', 'two', 'three', 'four', 'five']




```python
our_lists.pop(2)
```




    'three'




```python
our_lists
```




    ['one', 'two', 'four', 'five']




```python
popped_item=our_lists.pop(2)
```


```python
popped_item
```




    'four'




```python
our_lists
```




    ['one', 'two', 'five']




```python
new_list=["a","e","x","b","c"]
num_list=[4,1,8,3]
```


```python
new_list.sort()
```


```python
new_list
```




    ['a', 'b', 'c', 'e', 'x']




```python
num_list.sort()
```


```python
num_list
```




    [1, 3, 4, 8]



The .sort function does not actually return anything to assign as it occurs in place, so you can't assign a variable to this function. It will resort in a NoneType. See below for the correct way to assign a variable to a sorted list.


```python
new_list.sort()
sorted_list=new_list
```


```python
sorted_list
```




    ['a', 'b', 'c', 'e', 'x']




```python
num_list.reverse()
```


```python
num_list
```




    [8, 4, 3, 1]




```python
test_list=[2,9,5,1]
```


```python
test_list.reverse()
```


```python
test_list
```




    [1, 5, 9, 2]



.reverse function does NOT sort the list into order in reverse, it just reverses the current order. See below for example on how to sort and reverse.


```python
test_list.reverse()
```


```python
test_list
```




    [2, 9, 5, 1]




```python
test_list.sort()
test_list.reverse()
test_list
```




    [9, 5, 2, 1]




```python
test_list
```




    [9, 5, 2, 1]




```python
second_list=[5,2,9]
second_list.sort()
second_list.reverse()
second_list
```




    [9, 5, 2]




```python
test_list
```




    [9, 5, 2, 1]




```python
test_list.sort()
```


```python
test_list
```




    [1, 2, 5, 9]




```python
test_list.reverse()
```


```python
test_list
```




    [9, 5, 2, 1]




```python
nested_list=[1,2,3,[4,5]]
```


```python
nested_list
```




    [1, 2, 3, [4, 5]]




```python
nested_list=1,2,3,[4,5]
```


```python
nested_list
```




    (1, 2, 3, [4, 5])




```python
nested_list[
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[92], line 1
    ----> 1 nested_list[[1]]


    TypeError: tuple indices must be integers or slices, not list



```python

```
