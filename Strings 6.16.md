```python
'hello'
```




    'hello'




```python
"this is also a string"
```




    'this is also a string'




```python
"I'm going on a run"
```




    "I'm going on a run"




```python
2***2
```


      Cell In[4], line 1
        2***2
           ^
    SyntaxError: invalid syntax




```python
2**2
```




    4




```python
print("hello")
```

    hello



```python
print("hello world one")
print("hello world two")
```

    hello world one
    hello world two



```python
print('hello \n world')
```

    hello 
     world



```python
print('hello \nworld')
```

    hello 
    world



```python
print('hello \tworld')
```

    hello 	world


\t inserts a tab; \n creates a new line - these are escape functions


```python
len('hello')
```




    5




```python
len('hello world')
```




    11




```python
mystring = "Hello World"
```


```python
mystring
```




    'Hello World'




```python
mystring[0]
```




    'H'




```python
mystring[8]
```




    'r'




```python
mystring[-2]
```




    'l'



indexing - first character/space is 0 and counts up moving to the right, or start with -1 on the left and decrease to the left


```python
mystring
```




    'Hello World'




```python
mystring = "abcdefghijk"
```


```python
mystring
```




    'abcdefghijk'




```python
mystring[2:]
```




    'cdefghijk'




```python
mystring[:3]
```




    'abc'



slicing - [a:b:c] a=start (can leave blank if 0) b=stop (does NOT include the stop character) c=step (how many characters to "jump", kind of like skip counting; can also use -1 to reverse string by jumping *back* 1 number at a time). You don't have to include a number in each spot, it can just be :: or 3: or :3 or ::3. [0:] will include everything from the first number on because there is no stop included.


```python
mystring[2:5]
```




    'cde'




```python
mystring[7:9]
```




    'hi'




```python
mystring[::]
```




    'abcdefghijk'




```python
mystring[::2]
```




    'acegik'




```python
mystring[2:9:2]
```




    'cegi'




```python
mystring[::-1]
```




    'kjihgfedcba'




```python
"My name is Tiffany"[-5]
```




    'f'




```python
name="Sam"
```


```python
name
```




    'Sam'



Change "Sam" to "Pam" - name[0]='P' will return an error, instead, do as below using concatination to merge two strings together


```python
name[1:]
```




    'am'




```python
last_letters=name[1:]
```


```python
last_letters
```




    'am'




```python
"P"+last_letters
```




    'Pam'




```python
x="Hello World"
```


```python
x
```




    'Hello World'




```python
x=x+ " it is beautiful outside!"
```


```python

```


```python
x
```




    'Hello World it is beautiful outside! it is beautiful outside!'




```python
x="My name is Tiffany"
```


```python
y=" and I have six kids"
```


```python
x+y
```




    'My name is Tiffany and I have six kids'




```python
z=x+y
```


```python
z
```




    'My name is Tiffany and I have six kids'




```python
z[15:]
```




    'any and I have six kids'




```python
z[-15]
```




    'I'




```python
z[-15:]
```




    'I have six kids'




```python
z[10:19]+z[8:11]+z[0:3]+z[3:8]
```




    ' Tiffany is My name '




```python
letter="z"
```


```python
letter
```




    'z'




```python
letter*10
```




    'zzzzzzzzzz'




```python
2+3
```




    5




```python
"2"+"3"
```




    '23'



Concatination will not add strings that are numbers!


```python
x="Hello World"
```


```python
x
```




    'Hello World'




```python
x.upper()
```




    'HELLO WORLD'




```python
x= x.upper()
```


```python
x
```




    'HELLO WORLD'




```python
x=x.lower()
```


```python
x
```




    'hello world'




```python
x.upper
```




    <function str.upper()>



^ must include open and close parentheses or functions wont work - also functions are not scriptable (can't do x.upper[5:]


```python
x.split()
```




    ['hello', 'world']




```python
x="Hi my name is tiffany"
```


```python
x
```




    'Hi my name is tiffany'




```python
x.split("i")
```




    ['H', ' my name ', 's t', 'ffany']




```python
x.split(" ")
```




    ['Hi', 'my', 'name', 'is', 'tiffany']



.split can be used to create lists from strings (see above)


```python
my_name="Tiffany"
```


```python
print("Hello"+ my_name)
```

    HelloTiffany



```python
print("Hello"+" "+my_name)
```

    Hello Tiffany



```python
print("This is a string {}".format("INSERTED"))
```

    This is a string INSERTED



```python
print("The {} {} {}".format("fox","brown","quick"))
```

    The fox brown quick



```python
print("The {2} {1} {0}".format("fox","brown","quick"))
```

    The quick brown fox



```python
print("The {0} {0} {0}".format("fox","brown","quick"))
```

    The fox fox fox



```python
print("The {q} {b} {f}".format(f="fox",b="brown",q="quick"))
```

    The quick brown fox



```python
result=100/777
```


```python
result
```




    0.1287001287001287




```python
print("The result was {r}".format(r=result))
```

    The result was 0.1287001287001287



```python
print("The result was {r:1.3f}".format(r=result))
```

    The result was 0.129


Float formatting - {value:width.precision f} example above says value = r, width = 1, precision = 3 past decimal


```python
print("The result was {r:10.3f}".format(r=result))
```

    The result was      0.129



```python
print("The result was {r:50.3f}".format(r=result))
```

    The result was                                              0.129



```python
result=104.12342
```


```python
result
```




    104.12342




```python
print("The result was {r:1.4f}".format(r=result))
```

    The result was 104.1234



```python
name="Jose"
```


```python
print(f"Hello, his name is {name}")
```

    Hello, his name is Jose


f string (formatted string literals) - insert f in front of string to insert variable directly and can use multiple variables


```python
name="Sam"
age="3"
```


```python
print(f"{name} is {age} years old")
```

    Sam is 3 years old



```python

```
