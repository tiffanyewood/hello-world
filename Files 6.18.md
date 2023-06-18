This method ONLY works in Jupyter notebook 


```python
%%writefile myfile.txt
Hello this is a text file
this is the second line
this is the third line
```

    Writing myfile.txt



```python
myfile=open("myfile.txt")
```


```python
myfile=open("anotherfile.txt")
```


    ---------------------------------------------------------------------------

    FileNotFoundError                         Traceback (most recent call last)

    Cell In[3], line 1
    ----> 1 myfile=open("anotherfile.txt")


    File ~/anaconda3/lib/python3.10/site-packages/IPython/core/interactiveshell.py:282, in _modified_open(file, *args, **kwargs)
        275 if file in {0, 1, 2}:
        276     raise ValueError(
        277         f"IPython won't let you open fd={file} by default "
        278         "as it is likely to crash IPython. If you know what you are doing, "
        279         "you can use builtins' open."
        280     )
    --> 282 return io_open(file, *args, **kwargs)


    FileNotFoundError: [Errno 2] No such file or directory: 'anotherfile.txt'



```python
pwd
```




    '/Users/tiffanywong/Desktop/Python'



^pwd means Print Working Directory and tells you the file path for the file you are currently working in


```python
myfile=open("myfile.txt")
```


```python
myfile.read()
```




    'Hello this is a text file\nthis is the second line\nthis is the third line\n'




```python
myfile.read()
```




    ''



^.read() doesn't work again until you reset the cursor. Basically it has "read" the txt file and the cursor is now at the end so there is nothing else to return. See below.


```python
myfile.seek(0)
```




    0



^this resets the cursor to position 0


```python
myfile.read()
```




    'Hello this is a text file\nthis is the second line\nthis is the third line\n'




```python
contents=myfile.read()
```


```python
contents
```




    ''




```python
myfile.seek(0)
```




    0




```python
contents
```




    ''




```python
contents=myfile.read()
```


```python
contents
```




    'Hello this is a text file\nthis is the second line\nthis is the third line\n'




```python
myfile.seek(0)
```




    0




```python
myfile.readlines()
```




    ['Hello this is a text file\n',
     'this is the second line\n',
     'this is the third line\n']



Opening files in other locations:
Windows uses double \\ so python doesn't treat the second \ as an escape character
    myfile=open("C:\\Users\\UserName\\Folder\\myfile.txt")
Mac and Linux use / instead
myfile=open("/Users/YourUserName/Folder/myfile.txt")


```python
pwd
```




    '/Users/tiffanywong/Desktop/Python'




```python
myfile.close()
```


```python
with open("myfile.txt") as my_new_file:
    contents=my_new_file.read()
```


```python
contents
```




    'Hello this is a text file\nthis is the second line\nthis is the third line\n'



^If you just open a file, you have to close it first (see line 19). Otherwise if you try to open it later you'll get an error that Python is using this file still. To avoid this use line 21 command to open the file.


```python
with open("myfile.txt",mode="r") as myfile:
    contents=myfile.read()
```


```python
contents
```




    'Hello this is a text file\nthis is the second line\nthis is the third line\n'




```python
%%writefile my_new_file.txt
ONE ON FIRST
TWO ON SECOND
THREE ON THIRD
```

    Writing my_new_file.txt



```python
with open("my_new_file.txt",mode="r") as f:
    print(f.read())
```

    ONE ON FIRST
    TWO ON SECOND
    THREE ON THIRD
    



```python
with open("my_new_file.txt",mode="a") as f:
    f.write("FOUR ON FOURTH")
```


```python
with open("my_new_file.txt",mode="r") as f:
    print(f.read())
```

    ONE ON FIRST
    TWO ON SECOND
    THREE ON THIRD
    FOUR ON FOURTH



```python
with open("my_new_file.txt",mode="r") as my_new_file:
    contents=my_new_file.read()
```


```python
contents
```




    'ONE ON FIRST\nTWO ON SECOND\nTHREE ON THIRD\nFOUR ON FOURTH'



mode="a" is appending the file, meaning it is adding to the END of the file. You may need to use \n to create a new line


```python
with open("newwritingfile.txt",mode="w") as f:
    f.write("I CREATED THIS FILE!")
```


```python
with open("newwritingfile.txt",mode="r") as f:
    print(f.read())
```

    I CREATED THIS FILE!



```python
with open("anotherfile.txt",mode="w") as x:
    x.write("I made this.")
```


```python
with open("anotherfile.txt",mode="r") as x:
    print(x.read())
```

    I made this.



```python

```
