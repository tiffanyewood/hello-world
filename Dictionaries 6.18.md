Dictionaries use curly braces and colons to signify keys/values. Ex: ["key1":"value1","key2":"value2"]
Dictionaries are unordered and not sorted and are good to use when you don't know the actual location. BUT you can't sort, index, or slice it like a list. Keys should ALWAYS be strings.


```python
my_dict={"key1":"value1","key2":"value2"}
```


```python
my_dict
```




    {'key1': 'value1', 'key2': 'value2'}




```python
my_dict["key1"]
```




    'value1'




```python
price_lookup={"apple":2.99,"orange":1.99,"banana":0.99}
```


```python
price_lookup
```




    {'apple': 2.99, 'orange': 1.99, 'banana': 0.99}




```python
price_lookup['apple']
```




    2.99




```python
price_lookup["orange"]+price_lookup["banana"]
```




    2.98




```python
price_lookup["apple"]-price_lookup["orange"]+price_lookup["banana"]
```




    1.9900000000000002




```python
price_lookup["apple"]-(price_lookup["orange"]+price_lookup["banana"])
```




    0.010000000000000231




```python
d={"k1":123,"k2":[0,1,2],"k3":{"insideKey":100}}
```


```python
d
```




    {'k1': 123, 'k2': [0, 1, 2], 'k3': {'insideKey': 100}}




```python
d["k2"]
```




    [0, 1, 2]




```python
d["k3"]["insideKey"]
```




    100




```python
d["k2"][2]
```




    2




```python
d={"k1":["a","b","c"],"k2":[1,2,3]}
```


```python
d["k2"][2]
```




    3




```python
mylist=d["k1"]
```


```python
mylist
```




    ['a', 'b', 'c']




```python
letter=mylist[2]
```


```python
letter
```




    'c'




```python
letter.upper()
```




    'C'




```python
d["k1"][2].upper()

```




    'C'




```python
d={"k1":100,"k2":200}
```


```python
d["k3"] = 300
```


```python
d
```




    {'k1': 100, 'k2': 200, 'k3': 300}




```python
d["k1"]+d["k2"]
```




    300




```python
d={'k1': "100", 'k2': 200, 'k3': 300}
```


```python
d["k1"]+d["k2"]
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    Cell In[44], line 1
    ----> 1 d["k1"]+d["k2"]


    TypeError: can only concatenate str (not "int") to str


^numbers in quotes are STRINGS and not considered numbers. Numbers without quotes are numbers and can be used in math.


```python
d["k2"]=150
```


```python
d
```




    {'k1': '100', 'k2': 150, 'k3': 300}




```python
d={'k1': "100", 'k2': 200, 'k3': 300}
```


```python
d
```




    {'k1': '100', 'k2': 200, 'k3': 300}




```python
d.keys()
```




    dict_keys(['k1', 'k2', 'k3'])




```python
d.values()
```




    dict_values(['100', 200, 300])




```python
d.items()
```




    dict_items([('k1', '100'), ('k2', 200), ('k3', 300)])



^items are returned in parantheses and these are called tuples


```python
print(d)
```

    {'k1': '100', 'k2': 200, 'k3': 300}



```python

```


```python

```
