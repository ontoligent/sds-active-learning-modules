## Q1 

(1.0 points) Consider this function:

```python
def make_bigger(txt):
	new_txt = txt.upper()
    return new_txt
```

Which of these is a correct function call?

A. `make_bigger['somethingInTheWaySheMoves']` \
B. `'somethingInTheWaySheMoves'.make_bigger()` \
*C. `make_bigger('somethingInTheWaySheMoves')` \
D. none of these 


## Q2 

(1.0 points) True or False: Default arguments must follow non-default arguments.

*A. True \
B. False

## Q3

(1.0 points) Python functions require a return statement

A. True \
*B. False

## Q4

(1.0 points) Consider this function:  

```python
def commute_to_work(w, x):
    a = 10
    out = a * w + x
    return out
```

For all given values of `c` and `d`, where `c` and `d` are NOT EQUAL, do the following function calls produce equivalent results?

A. yes \
*B. no \
C. cannot be determined 

#Note: Gven that `c` and `d` are not equal,permuting the order will produce different function outputs. Thus the results will NOT produce equivalent results. 

## Q5

(1.0 points) Functions should (select all that apply):

*A. Do one thing \
*B. Have a good name \
*C. Contain a docstring \
D. Be shorter than ten lines in length


## Q6

(1.0 points) What does this return? `(lambda x: 1 - x%2)(5)`

A. an error\
B. 1\
C. 5\
*D. 0

## Q7

(1.0 points) What does this code block print?  

```python
def gamma(x):
    if x < 10:
        return(0)
    elif x == 10:
        return(x**2)
    return(1)
y = gamma(20)
print(y)
```

A. 0 \
B. 400 \
*C. 1 \
D. an error 


## Q8 

(1 point) Recursive functions can often be replaced by code blocks that use a looping operation (e.g. for or while statement).

*A. True \
B. False

## Q9

(1 point) Which of the following are good reasons to define groups of functions that call each other and share data?

*A. Functions often are designed to solve a common problem.\
*B. Complex functions should be broken up into simpler and reusable functions \
*C. Functions often perform different roles in a program, such as apply a mathematical formula or interact with a user. \
D. Functions must return values, and these values need to be used somehow

## Q10

(1 point) Which of the following are true statements about how Python handles variable scope in functions?

A. Functions can never see variables defined outside of them.\
*B. Unless a variable is declared to be global within a function, a variable is considered local to a function if that variable is assigned a
value in the function. \
C. Code outside of a function may see variables defined inside of a function. \
*D. A name, such as `x` , can refer to many different variables in a program.


