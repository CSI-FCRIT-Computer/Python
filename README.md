# Cryptex Python 2021

# Day 1

# Introduction to Python Programming

![](https://i.pinimg.com/originals/f0/57/45/f05745097ea6273709bfe2e727989488.jpg)

## Input and Output

    a=input()
    print(a)

## Variable

A variable is an identifier for a memory location in which data can be stored and subsequently recalled.

Variables are used for holding data values so they can be utilized in various computations in a program.

In python, we can declare variables in following way :

    x = 5
    y = "Michael Scott"
    z = 3.50
    print(x)
    print(y)
    print(z)

The data stored in the variables has a certain type.

For Example :-

str : String

int : integer

float : decimals till 7 decimal digit precision

complex : complex numbers

boolean : True or False

We will learn more about data and structures of data shortly.

#### Checking the data type of the given variable :

we use type() function

    print(type(x))

## Python Casting

![](https://www.codeitbro.com/wp-content/uploads/2020/07/python-funny-meme-17-cant-compare-int-and-float.jpg)

At times when we need to specify a certain variable to a particular datatype, we use _casting_.

    x = int(5.4)
    y = str(1.2)
    z = float(9)
    print(x)
    print(y)
    print(z)

## Operators

Data saved in the variables can be operated on.

There are 7 types of operators :

#### Arithmetic Operators:

Addition, Subtraction, Multiplication, Division, Floor division, Exponentiation, Modulus.

    x = 5
    y = 10
    print(x+y)
    print(x-y)
    print(x*y)
    print(x/y)#normal divison
    print(x//y)# floor division
    print(x^3)
    print(x%y)

#### Assignment Operators :

    x = 5
    #assigns value 5 to the variable x
    x += 5
    # x = x + 5
    # Similarly we can use it with other arithmetic operators.

### Note:

![](https://pics.onsizzle.com/when-you-write-i-in-a-python-code-we-dont-63760085.png)

#### Comparison Operators :

    x != y
    #x not equal to y

    x == y
    #x equal to y

    x > y
    #x greater than y

    x >= y
    # x greater than or equal to y

    x < y
    #x less than y

    x <= y
    #x lesser than or equal to y

#### Logical Operators :

    x < 20 and y < 30
    x > 34 or y > 21
    not(x > 7 and y < 0)

#### Identity Operators :

    x = 5
    y = 10
    print(x is y)
    print(x is not y)

#### Membership Operators :

    x in y
    #returns if certain data labelled x is present in the structure y
    x not in y

#### Bitwise Operators :

    x&y
    x|y
    x^z
    ~x
    x<<
    x>>

## Diving in Python!

![](https://i.imgflip.com/5m10n4.jpg)

Like every spoken and written language, similarly we have syntax for programming languages too.

Python has relatively easier syntax in comparison to other languages likes C, C++, Java.

Python is a high level language.

_It is used for web development, AI, ML, Deep Learning, Image processing purposes._

Let's focus on the python syntax now.

1. Indentations

To put in simple words - space before beginning of code in every line of the program.

Python uses indentation to recognize particular block of code.

Example :

      x = 3

      if x == 3:

        print("yes")

Here assignment of 3 to x is a block while, if and then condition is another block.

![](https://pics.me.me/exit-programming-in-python-indentation-error-python-hitting-me-again-65730141.png)

2. Comment

When we write code, for future references we use commenting feature to understand what we had written in the past.

      ##this is an example of commenting in python

![](https://www.codeitbro.com/wp-content/uploads/2020/07/python-jokes-delete-block-of-code.jpg)

## Conditional Statements in Python

#### if

    Michael = 100
    Toby = 0

    if Michael > Toby :
      print('If I had a gun with two bullets and I was in a room with Hitler, Bin Laden, and Toby,I would shoot Toby twice.')\

![](https://pics.me.me/Instagram-6dcab8.png)

in case you just need to check if the condition holds, you can use pass.

    Jim = 100
    Roy = 0

    if Roy > Jim :
      pass

#### if else

    Michael = 10
    Jim = 9.5

    if Michael > Jim :
      print('Michael is better than Jim. ')
    else :
      print('Jim is better than Michael. ')

![](https://cdn3.whatculture.com/images/2016/02/vfl0yZYJ.jpg)

#### elif

    Dwight = 100
    Andy = 60

    if Dwight > Andy :
      print('Dwight is better manager than Andy')

    elif Dwight == Andy :
      print('This can never happen')

    else :
      print('Dwight will always be the best')

![](https://res.cloudinary.com/jerrick/image/upload/f_jpg,fl_progressive,q_auto,w_1024/e1ly8jom8drdzderu7qp.jpg)

#### Nested if

    Kevin = 42
    Angela = 12

    if Kevin > 40:
      if Angela == 12 :
        print('The office is the best show')
      else :
        print('Angela has 12 cats !')
    else :
      print('Your counting is horrible than Kevin')

![](https://media1.popsugar-assets.com/files/thumbor/eMD_e8DKh44QAlhtYdeAgZfSoYA/1065x113:2758x1806/fit-in/2048xorig/filters:format_auto-!!-:strip_icc-!!-/2019/04/26/862/n/1922283/2979532d5cc35efc8e2870.12777856_/i/Angela-Kinsey-Brian-Baumgartner-Interview-About-Office.jpg)

## Loops

To iterate through same line of code over and over again, we use loops. (Finite loops, if you don't want your computer to go gaga)

There are 3 types of loops :

#### For Loop

A for loop is used for iterating over a sequence.

With the for loop we can execute a set of statements, once for each item in a list, tuple, set etc.

    sum = 0
    for a in range(0,100,5):
      sum += a
    print(sum)

    #prints sum of numbers between 0, 100 at interval of 5.

#### While Loop

    a = 0
    while a < 20:
      print(a)
      a += 1

    #prints numbers from 0 to 19

![](https://ahseeit.com//king-include/uploads/2021/01/135621505_3490110337777630_2014426057131565060_n-5779826117.jpg)

#### Break Statement

With the break statement we can stop the loop even if the loop condition is true.

    b = 100
    while b < 1000 :
      print(b)
      if b == 120:
        print('loop reached till 120')
        break
      b += 1

#### Continue Statement

    c = 5
    for c in range(0,20):
      if c == 10 :
          print("we are at 10")
          continue
      print(c)

## Functions

Instead of re-writing same lines of code over and over again, we put the code in a function and callback the function.

![](https://i.pinimg.com/originals/c6/4e/fc/c64efc9adaedbf446f328698e8b67388.jpg)

In Python a function is defined using the def keyword

    def function_first(a):
      print("Happy Coding ", a)

    print("Input your name")
    abc = input(str())

    function_first(abc)

#### _Recursive Function_

Recursion is the process of defining something in terms of itself.

In Python, we know that a function can call other functions. It is even possible for the function to call itself. These types of construct are termed as recursive functions.

    ## only for positive and non zero numbers
    print("Number to calculate factorial")
    n = int(input())
    factorial(n)

    def factorial(x):
      fact = 1
      if x == 1:
        return x
      else :
        fact = factorial(x)*factorial(x-1)

![](https://i.redd.it/oxrtfir9rfa21.jpg)

# Data structures

#### List

[Python Data Structures Cheat Sheet - Aakash Yadav](https://aakashcode12.github.io/Python-Cheat-Sheet/)

Lists are used to store multiple items in a single variable.Lists can be used for any type of object, from numbers and strings to more lists.

They are accessed just like strings (e.g. slicing and concatenation) so they are simple to use and they’re variable length, i.e. they grow and shrink automatically as they’re used.

    l = ['element', 2, 'alphanumeric2021','python', 3,'cryptex', 'level up', '2019']

    ##experimenting with the list display options
    print(l[1])
    print(l[-2])
    print(l[3:])
    print(l[-1:2])

    ##checking if the element is present in the list
    if 'cryptex' in l :
      print('True')

    ## changing elements of the list
    string = input()
    l[0] = string
    print(l)

    ##inserting at certain position using insert
    l.insert(0, "Hello janta")
    print(l)

    ##adding elements to the list
    l.append('Mumbai')

    ##removing a particular element
    l.remove('2019')
    print(l)

    #using pop
    l.pop(3)
    print(l)

    #Clear list
    l.clear()

    #Sorting

    alpha = ['Aaditee', 'Aakash', 'Snehal','Laurel', 'Anushka', 'Bryan', 'Vardaan', 'Loukik', 'Elisha', 'Trevor', 'Unni', 'Shreya']

    alpha.sort()
    print(alpha)

    alpha.sort(reverse = True)
    print(alpha)

    ##making a copy of list
    copies = alpha.copy()

    ##joining two lists together
    beta = [1, 2, 3, 4]
    gamma = ['Hello', 'Hola', 'Namaste', 'Ram Ram']

    omega = beta + gamma
    print(omega)

    beta.extend(alpha)
    print(beta)

    for x in gammma:
      beta.append(x)
    print(beta)

![](https://www.codeitbro.com/wp-content/uploads/2020/07/python-funny-meme-6-lists.jpg)

![](https://i.redd.it/qv7nvc1vrop31.jpg)

#### Tuple

Tuples are used to store multiple items in a single variable.A tuple is a collection which is ordered and unchangeable. Tuples are written with round brackets.

    t = ('Ice bear', 'Trimmer', 'Anu Malik', 'Kermit Kardashian', 'Ab-norm-el', 'Golden Lighting', 'Billy Bonka', 'Dracorexia','Christo' )

    ##length of the tuple
    print(len(t))

    ##type
    print(type(t))

    ##accessing the tuple
    print(tuple[-3])

    ##range
    print(t[1:5])
    print(t[:3])
    print(t[2:])

    ##joining 2 Tuples
    T = ('computer', 'it', 'extc', 'electrical')

    tuple_3 = t + T
    print(tuple_3)

    tuple_4 = T*2

![](https://res.cloudinary.com/practicaldev/image/fetch/s--4cmlI56_--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ldnbot0l2a0ldm5bdilw.png)

#### Set

Sets are used to store multiple items in a single variable. Set is one of 4 built-in data types in Python used to store collections of data, the other 3 are List, Tuple, and Dictionary, all with different qualities and usage.

A set is a collection which is both unordered and unindexed. Sets are written with curly brackets.

    s = {"Babu Rao", "Raju", "Ghanshyam", "Anuradha", "Kachra Seth","Tiwari Bhai" }

    print(s)

    #length of set
    print(len(s))

    #type
    print(type(s))

    #accessing items
    for i in s:
      print(i)

    #adding new elements
    s.add('Phir Hera pheri')
    print(s)

    S = {'memes', '25 days', 'aye'}

    s.update(S)

    print(s)

    #removing items
    s.remove('Anuradha')

    print(s)

    #clearing the set
    S.clear()
    print(S)

    #operations on set
    set_1 = {'trump', 'narendra', 'Kim jun'}
    set_2 = {'Corrupt', 'Politics', 'Orange'}

    set_3 = set_1.union(set_2)

    print(set_3)

    set_1.update(set_2)

![](https://indianmemetemplates.com/wp-content/uploads/phir-hera-pheri-akshay-waiting-pose-.jpg)

#### Dictionary

Dictionary items are ordered, changeable, and does not allow duplicates.

Dictionary items are presented in key:value pairs, and can be referred to by using the key name.

![](https://benjdd.com/assets/memes/dictionary.jpg)

    d = {"Coding" : 1, "Debate" : 2, "Cryptex" : 3, "Introdcution to Engineering" : 4, "Acess" : 5, "Hacakthon" : 6, "Membership" : 7}

    print(d)

    print(len(d))

    print(type(d))

    x = d.keys()

    y = d.values()

    d.update({"LinkedIn" : 8})

    del d["Membership"]

    print(d)

    d.clear()
    print(d)

![](https://www.codeitbro.com/wp-content/uploads/2020/07/hilarious-python-meme-10-before-and-after-coding.jpg)
