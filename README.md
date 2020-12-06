# Python Exam Practice
---
*(Based on ENGINEER 1P13 computing material, written by Willie Pai)*

For more study material, view all previous Pre-Lab & In-Lab Jupyter Notebooks

### Topics Covered:

* Inputs and Outputs
* Built-in Functions
* Errors
* Defining and calling functions
* Passing Arguments
* Returning Values
* Variable Scope
* Lists
* String Operations
* For Loops
* Boolean Comparison Operators
* Decision Structures
* While Loops
* Opening/closing files 
* Reading & looping through files (Methods)  
* Writing & looping to files (Methods)
* Boolean Comparison Operators
* Decision Structures

#### Student resources

[Computing Notes by Quinn Ha](https://docs.google.com/document/d/1RuwBbcek9Xu1b7VQcDS375IIgzdB0hYu-BF0D8yqU7o/edit)

[Practice Quiz by peg](https://drive.google.com/file/d/18XUPfUog1fpsEUg33CCFG1tykJAse2BX/view?usp=sharing)

#### School resources

[1P13 Lab A Computing Review](https://drive.google.com/file/d/17sdQrqR8MnEBDfB4hLXShavCT5UH_AYo/view?usp=sharing)

#### Online resources

[2 Practice Quizzes from PythonSpot.com](https://pythonspot.com/python-tests-quizes/)

[Beginners Python Quiz](https://pynative.com/basic-python-quiz-for-beginners/)

[Operators and Expressions Quiz](https://pynative.com/python-operators-and-expression-quiz/)

[List Quiz](https://pynative.com/python-list-quiz/)

[If, Else and For Loop Quiz](https://pynative.com/python-if-else-and-for-loop-quiz/)

#### 1. What will the following code output?
```python
print(25 % 4)
```

A) `25/4`

B) `6.25`

C) `1`

D) `6`


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 2. What will the following code output?
```python
print(25 / 4)
```

A) `25/4`

B) `6.25`

C) `1`

D) `6`


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 3. What will the following code output?
```python
print(25 // 4)
```

A) `25/4`

B) `6.25`

C) `1`

D) `6`


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 4. Which output will this code produce?
```python
a = 1
b = 2
c = "3"

print(a + b + c)
```

A) `6`

B) `TypeError`

C) `33`

D) `123`


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 5. What will the following code output if the input `25` was given?
```python
first_value = input()
sum = first_value + str(3)
print(sum)
```

A) `253`

B) `8`

C) `TypeError`

D) `25 3`


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 6. Will the following code return True or False?
```python
print(not(True and False) or not(False and False))
```


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 9. Which of the following will return an error?

A) `print('def HelloWorld(string):')`

B) `print(str(input('int("Hello!"):')))`

C) `print (  "Hello World!"        )`

D) `print(13 + "years old")`


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 10. What will this code output?

```python
some_list = ["One", "Two", "Three", "Four", "Five"]

for word in some_list:
    word.strip('e').split()
    print(word)
```

A)
```python
On
Thr
Fiv
Svn
Nin
```
B)
```python
On
Thr
Fiv
Seven
Nin
```
C)
```python
['On']
['Thr']
['Fiv']
['Seven']
['Nin']
```
D)
```python
One
Three
Five
Seven
Nine
```
E)
```python
['O', 'n']
['T', 'h', 'r']
['F', 'i', 'v']
['S', 'e', 'v', 'e', n']
['N', 'i', 'n']
```


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 11. Which of the following _does not_ return an integer output of 3?
```python
a = [1, 10, 25]
b = ['bed', 'blanket', 'pillow']
c = [2, 'hi', [1, 2]]
```

A) `len(b[1].split()) + len(c) - a[0] `

B) `len(c[1]) - len(str(a[2])) + round(len(b[0]))`

C) `sum(c[2]) + b[2].index('l') - (a[2] % 11) + 1`

D) `c[2].index(2) - (a[1] / 10.0) + len(b[0])`


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 12. How many times will the string `Proceed` be printed?
```python
list_a = [2, 4, 6, 8]
list_b = [1, 3, 5, 9]

result = 0;

for i in list_a:
    for j in list_b:
        if i < j and i * j > result:
            result += 1
            print("Proceed")
```

A)    6 times

B)    7 times

C)    8 times

D)    9 times


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 13. Which of the following functions will print the integer 2021?

A)
```python
x = 2020

def modify():
    x = 2021
    global x
    return x
    
print(modify())
```

B)
```python
x = 2020

def modify(y):
    global x
    x = 2021
    return y
    
print(modify(x))
```

C)
```python
x = 2020

def modify(y):
    global x
    y = x
    x = 2021
    return(y)
    
modify(x)
print(x)
```

D)
```python
x = 2020

def modify(y):
    global x
    return y
    x = 2021
    return x

print(modify(x))
```


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 14. Which of the following functions returns a list of even numbers found inside a given list of integers?

A)
```python
def returnEven(list):
    even_numbers = []
    for i in range(list):
        if i % 2 == 0:
            even_numbers.append(i)
    return even_numbers
```

B)
```python
def returnEven(list):
    even_numbers = []
    for number in list:
        if i % 2 == 0:
            even_numbers += number
    return even_numbers
```

C)
```python
def returnEven(list):
    even_numbers = []
    for i in range(len(list)):
        if list[i] % 2 == 0:
            even_numbers.append(list[i])
        return even_numbers
```

D)
```python
def returnEven(list):
    even_numbers = []
    for number in even_numbers:
        if number % 2 == 0:
            even_numbers.append(number)
    return even_numbers
```


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 15. Which follow code outputs the same result as this for loop?
```python
for i in range(10):
    i += 2
    print(i)
```

A)
```python
x = 10
while x < 30:
    print(int(x / 2 - 3))
    x += 2
```

B)
```python
x = 2
while x <= 12:
    print(x)
    x += 1
```

C)
```python
x = 2
while x < 12:
    x += 1
    print(x)
```

D)
```python
x = 0
while x > 12:
    print(x)
    x += 1
```


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 16. True or False: In Python, a variable must be declared before it is assigned a value.


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 17. True or False: The ‘in’ operator is used to check if a value exists within an iterable object container such as a list. Evaluates to true if it finds a variable in the specified sequence and false otherwise.


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 18. True or False: Not writing a `return` statement inside of a function will result in an error


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 19. True or False: Tuples are mutable data types; lists are immutable data types


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 20. Given a text file, `document.txt`, that has the following text:

```python
['A', 1]
['B', 2]
['C', 3]
['D', 4]
['E', 5]
```

#### What will the following code output?

```python
file = open("document.txt", 'r')

for line in file.readlines():
    print(line[1])

file.close()
```

A)
```python
1
2
3
4
5
```

B)
```python
"1"
"2"
"3"
"4"
"5"
```

C)
```python
'
'
'
'
'
```

D)
```python
A
B
C
D
E
```


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 21. Given a text file, `document.txt`, that has the following text:
```
One A
Two B
Three C
Four D
Five E
```
#### Where each line is a string and an integer seperated by a space (" ").

#### Which code will give the following output?
```python
One
A
Two
B
Three
C
Four
D
Five
E
```

A)
```python
file = open("document.txt", 'r')
for line in file.readlines():
    print(line)
file.close()
```

B)
```python
file = open("document.txt", 'r')
for line in file.readlines():
    print(line)
    line = file.readline()
    print(line)
file.close()
```

C)
```python
file = open("document.txt", 'r')
line = file.readline()
while line != "":
    line.split()
    print(line[0])
    print(line[1])
file.close()
```

D)
```python
file = open("document.txt", 'r')
line = file.readline()
while line != "":
    print(line.split()[0] + "\n" + line.split()[1])
    line = file.readline()
file.close()
```


```python
# Your answer: 
# TEST YOUR CODE HERE
```

#### 22. Given a function definition explaining the purpose of the function, rewrite the function to correct its error.
```python
def divideByTwo(numbers):
    '''
    Given a list of integers, return a list of floats containing half the value of each integer
    '''
    half_numbers = []
        for num in numbers:
        half_num = num / 2
    half_numbers.append(num)
    return half_numbers
```

```python
Double click to write your answer here in this cell. Don't delete the ``` marks.
```
