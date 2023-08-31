# M02 In-Class Exercises

DS 5100 | Summer 2023 | Residential

# Exercise 2.1

Define a string with a length `>= 6` and print:
- the first three characters of the string
- the last three characters of the string


```python
mystr = 'python'
len(mystr) >= 6
```




    True




```python
print(mystr[:3])
print(mystr[-3:])
```

    pyt
    hon


# Exercise 2.2

Create a new list and assign three values to it. 

Then print the second element from the list.


```python
mylist = []
mylist.append('first')
mylist.append('second')
mylist.append('third')
print(mylist[1])
```

    second



```python
mylist = []
mylist += ['first']
mylist += ['second', 'third']
print(mylist[1])
```

    second



```python
mylist2 = []
```


```python
mylist2[0] = 'foo'
```


    ---------------------------------------------------------------------------

    IndexError                                Traceback (most recent call last)

    Cell In[2], line 1
    ----> 1 mylist2[0] = 'foo'


    IndexError: list assignment index out of range



```python
mylist = ['first','second','third']
print(mylist[1])
```

    second


# Exercise 2.3

Create to a tuple with three values.

Then, try to append a fourth value. 


```python
mytuple = 1, 2, 3
```


```python
mytuple = (1, 2, 3)
```


```python
mytuple = tuple([1, 2, 3])
```


```python
mytuple.append(4)
```


    ---------------------------------------------------------------------------

    AttributeError                            Traceback (most recent call last)

    Cell In[9], line 1
    ----> 1 mytuple.append(4)


    AttributeError: 'tuple' object has no attribute 'append'


# Exercise 2.4

Assign a value to a string.

Assign three string values to a set.

Check if the string is in the set.


```python
val = 'ERROR'
levels = {'WARN','ERROR','CRITICAL'}
```


```python
val in levels
```




    True




```python
levels = {'WARN','ERROR','CRITICAL','WARN','ERROR','CRITICAL'}
```


```python
levels
```




    {'CRITICAL', 'ERROR', 'WARN'}



# Exercise 2.5

Create a dictionary containing at least three key-value pairs.

Use `get()` to index into the dictionary with one of the keys to extract the corresponding value.

Then, store the keys in a list and print the list.


```python
name_age = {
    'greg': 15, 
    'annabel': 22, 
    'joaquin': 19
}
```


```python
print('name_age[joaquin] =', name_age.get('joaquin'))
```

    name_age[joaquin] = 19



```python
names = list(name_age.keys())
```


```python
print('names:', names)
```

    names: ['greg', 'annabel', 'joaquin']



```python
type(name_age.keys()), type(names)
```




    (dict_keys, list)



# Exercise 2.6

Convert the following sentence into a set of lowercase words sorted alphabetically.

Do not include the punction mark in the resulting set.

`"The quick brown fox jumped over the lazy dogs."`



```python
mystring = "The quick brown fox jumped over the lazy dogs."
```


```python
mystring1 = mystring.replace('.', '')
mystring2 = mystring1.lower()
mystring3 = mystring2.split()
myset1 = set(mystring3)
myset2 = sorted(myset1)
```


```python
myset2
```




    ['brown', 'dogs', 'fox', 'jumped', 'lazy', 'over', 'quick', 'the']




```python
sorted(mystring3)
```


```python
sorted(set(mystring.replace('.', '').lower().split())
```




    ['brown', 'dogs', 'fox', 'jumped', 'lazy', 'over', 'quick', 'the']



# Exercise 2.7 

Compare the lengths of the preceding list and set. 

If not equal, give the difference.


```python
mylist = mystring.replace('.', '').lower().split()
myset = set(mylist)
```


```python
len(mylist) == len(myset)
```




    False




```python
abs(len(mylist) - len(myset))
```




    1



# Exercise 2.8

Define three variables of any type.

Use an `f` string to print a string containing each variable name followed by its value, using comma separators between the pairs.

For example:

`epoch 1, mode TRAIN, ...`


```python
epoch = 1
mode = "TRAIN"
loss = 0.46

print(f"epoch {epoch}, mode {mode}, loss {loss}")
```

    epoch 1, mode TRAIN, loss 0.46


# Exercise 2.9

Define two variables, assigning them floating point values. 

Write an expression using an operation on the two variables that will produce a value that may be cast as an integer. 

Next, use a logical operation that uses the integer that evaluates to `False`. Print the result with `print()`


```python
var1 = 1.5
var2 = 20.5
var3 = int(var1 // var2)
```


```python
var1 // var2
```




    0.0




```python
var3
```




    0




```python
test = var3 < 0
```


```python
print(test)
```

    False


# Exercise 2.10

Write a Python program to print the input string in the format of the output:

Input:

“Twinkle, twinkle, little star, How I wonder what you are! Up above the world so high, Like a diamond in the sky. Twinkle, twinkle, little star, How I wonder what you are”

Output:

```
Twinkle, twinkle, little star,
	How I wonder what you are! 
		Up above the world so high,   		
		Like a diamond in the sky. 
Twinkle, twinkle, little star, 
	How I wonder what you are
```

## Solution 1


```python
print("Twinkle, twinkle, little star, \n\tHow I wonder what you are! \n\t\tUp above the world so high, \n\t\tLike a diamond in the sky. \nTwinkle, twinkle, little star, \n\tHow I wonder what you are!")
```

    Twinkle, twinkle, little star, 
    	How I wonder what you are! 
    		Up above the world so high, 
    		Like a diamond in the sky. 
    Twinkle, twinkle, little star, 
    	How I wonder what you are!


## Solution 2


```python
msg = """
Twinkle, twinkle, little star, 
\tHow I wonder what you are! 
\t\tUp above the world so high, 
\t\tLike a diamond in the sky. 
Twinkle, twinkle, little star, 
\tHow I wonder what you are!
"""
```


```python
print(msg)
```

    
    Twinkle, twinkle, little star, 
    	How I wonder what you are! 
    		Up above the world so high, 
    		Like a diamond in the sky. 
    Twinkle, twinkle, little star, 
    	How I wonder what you are!
    


# Exercise 2.11

Compute `a` and `b` as follows:

```python
a = 0.15 + 0.15
b = 0.1 + 0.2
```

Test to see if `a` and `b` are equal.


```python
a = 0.15 + 0.15
b = 0.1 + 0.2
```


```python
a == b
```




    False




```python
a, b
```




    (0.3, 0.30000000000000004)



What is going on? Floating point comparisons are unreliable because of the way the computer stores their values.

Accoring to [The Floating-Point Guide](https://floating-point-gui.de/errors/comparison/), "Due to rounding errors, most floating-point numbers end up being slightly imprecise."
