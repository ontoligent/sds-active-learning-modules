# Quiz 

## Q1. 

(1.0 points) In Python the bodies of if/else statements, for loops, and while loops need to be properly and consistently indented. Is this statement true or false?

*A. True\
B. False

## Q2. 

(1.0 points) It is _________ to embed a for-loop in the body of an if-statement. (Pick an option to complete this sentence that makes the statement true.)
 
A. impossible \
B. syntactically incorrect \
*C. syntactically correct \
D. syntactically correct but not advised

## Q3. 

(1.0 points) Which of the following statements is true about ?else? and `elif` in the context of Python control structures?

*A. `elif` needs a condition, whereas ?else? does not\
B. `elif` and ?else? are both used as catch-alls after a sequence of if-statements where all conditions are not met\
C. `elif` is a general catch-all whereas ?else? is not\
D. `elif` and ?else? cannot show up together in a code segment used for conditional processing

## Q4. 

(1.0 points) Review the following code snippet. What is the output? 

```python
var1 = 1
while var1 < 10:
    var1 = var1 * 2
    if var1 == 4:
        continue
    if var1 == 6:
        break
print(var1)
```

A. 2 \
B. 4 \
C. 6 \
*D. 16 

## Q5. 

(1.0 points) Generally, a for-loop is used when the number of iterations is known ahead of time (e.g. iterating over an iterable like a list of items or iterating a specific number of times) whereas a while-loop will iterate until a particular condition is met and it might not be apparent how many iterations will occur. Is this statement true or false?

*A. True\
B. False

## Q6. 

(1.0 points) What is the output of the following code, if $n = 10345$?

```python
length = 0
while n > 0:
 n //= 10 # this is equivalent to n = n // 10
 length += 1
print(length)
```

A. 0 \
B. 3 \
C. 4 \
*D. 5

## Q7. 

(1.0 points) An iterator knows when it is at the end of the iterable object and therefore, you can call the next() method (which gets the next item from the iterator) as many times as you want, and it will not be a problem since it will always stop once it runs out of items to retrieve. Is this statement true or false?\

A. True\
*B. False

## Q8. 

(1.0 points)

What does the following code print?

```python
powers = [2,4,8,16,32,64]
some_vals = [int(x/2) for x in powers if x < 10]
print(some_vals)
```

A. `[2, 4, 8]` \
*B. `[1, 2, 4]` \
C. `[1, 2, 4, 8, 16, 32]` \
D. none of these \

## Q9. 

(1.0 points)

What does the following code print?

```python
codedMessage = '.GERYEXAKTL!'
decodedMessage = [char for index, char in enumerate(codedMessage)
 if (index % 2 == 1)]
print(decodedMessage)
```

A. `['.','G','E','R','Y','E','X','A','K','T','L','!']` \
B. `['G']` \
*C. `['G', 'R', 'E', 'A', 'T', '!']` \
D. `['.', 'E', 'Y', 'X', 'K', 'L']` \
E. `['G', 'R', 'E', 'Y', '!']`

## Q10. 

(1.0 points) Which of these are true statements about list comprehensions? Select all that apply:

*A. they produce a list\
B. they must contain a while-loop\
*C. they contain a for-loop\
*D. they may contain one or more if-statements
