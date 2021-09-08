# Day 2


### Problems - Python

#### print a list

    a=[1,2,3,4,5]
    for i in a:
      print(i)
    # in a single line
    print(*a)


#### 1. Input 4 integers in a single line and print them. Also, perform sum of those integers



    input_string = input()
    list_a = input_string.split()
    list_b=[]
    for i in list_a:
      list_b.append(int(i))

    print(type(list_b[0]))
    print(sum(list_b))


#### 2.Find Cardinal Values in a list (remove duplicates)
   
    list_A = [5,5,5,3,3,1]
    set_A= set(list_A)
    print(set_A)
    print(list(set_A))


#### 3. Write a Python program to compute the difference between two lists.
* Sample data: ["red", "orange", "green","blue",white"]
* ["black", "yellow", "green", "blue"]
* Expected Output:
* Color1-Color2: ['white', 'orange', 'red']
* Color2-Color1: ['black', 'yellow']


    a=[1,2,3,4]

    b=[2,3,5,97]

    a=list(set(a)-set(b))
    print(a)

#### 4. Generate the A.P in a list
##### where a=4, d=5 for n=5

    l=[]
    a=4
    for i in range(5):
      l.append(a)
      a+=5

    print(l)

#### Fibonacci Series (first 10 elements)

    a=1
    b=1
    print(a)
    print(b)
    
    count = 8
    while(count>0):
      c=a+b
      print(c)
      a=b
      b=c
      count-=1




#### [Hackerrank Problem - Mutations](https://www.hackerrank.com/challenges/python-mutations/problem)

#### Yesterday's Factorial Recursion Problem

    def factorial(n):
      if n == 0:
        return 1
      else:
        return n * factorial(n - 1)
        
    print(factorial(5))


### Object Oriented Programming in Python (OOPS)

![](https://miro.medium.com/max/500/1*-dmHYcAiphpWe6m0pcd-AA.png)

### 5.  Classes and Objects

![](https://media.geeksforgeeks.org/wp-content/cdn-uploads/20190501121513/inheritance.png)
![](https://miro.medium.com/max/1200/1*LNe8barKrwOGyNFY0mPfuA.jpeg)


A class is a user-defined blueprint or prototype from which objects are created.

#### Class and Objects Code in Python

    class Car:
        def Engine(self):
            print("Yeah I have good engine boom boom") 

    a = Car()
    a.Engine()

    
<hr>

### 6.  Inheritance
![](https://img.devrant.com/devrant/rant/r_403541_YuG5k.jpg)

![](/memes/unnamed.jpg)

When a **child class** inherits properties from a **parent class**, this property is known as inheritance. 


#### Single Inheritance

![](https://iq.opengenus.org/content/images/2019/05/Single.png)

    class Car:
        def Engine(self):
            print("Engine sound goes grooooooom")

        def Horn(self):
            print("honk honk honk")


    class Ciaz(Car):
        def GoodLooks(self):
            print("Yeah I have good looks")


    a = Ciaz()

    a.Engine()
    a.Horn()
    a.GoodLooks()

#### Multiple Inheritance

![](/memes/multipleinheritance.png)

    class Car:
        def Engine(self):
            print("Engine sound goes grooooooom")

        def Horn(self):
            print("honk honk honk")


    class Plane:
        def Aero(self):
            print("Yeah I have aerodynamics")


    class BMW_M3(Car, Plane):
        def Speed(self):
            print("I have speed yeah")


    obj_from_bmwm3 = BMW_M3()

    obj_from_bmwm3.Engine()
    obj_from_bmwm3.Horn()
    obj_from_bmwm3.Aero()
    obj_from_bmwm3.Speed()

<hr>


### 7.  Math Module

Future Reference: [w3schools link](https://www.w3schools.com/python/module_math.asp)

Math Module has **many functions**, we will touch a few functions and later I will give a question so that you also have to research on the topic.

#### GCD

    #Import math Library
    import math

    #find the  the greatest common divisor of the two integers
    print (math.gcd(3, 6))

#### Power

    # Import math Library
    import math

    #Return the value of 9 raised to the power of 3
    print(math.pow(9, 3))


![](https://thepukekopatch.files.wordpress.com/2020/04/0b64f-question.png)

### Construct the following equation in python 
![](/memes/range.png)
The program must take in values of u, tetha and g and give the R as output.

##### Hint: USE math library

    import math 

    u=5
    g=10
    tetha=50
    twice_tetha=2*tetha
    u_square=math.pow(u,2)

    range_projectile=(u_square*(math.sin(twice_tetha)))/g

    print(range_projectile)


<hr>



### 8. SMTP Library

#### Important Functions are:

    pip install smtp


1. server.login("email","pass")
2. server.sendmail("from","to","msg")
3. server.quit()



### 9.  Project on Email Sendig Using SMTP
#### Problem Statement: 
![](https://res.cloudinary.com/practicaldev/image/fetch/s--rN0fhOES--/c_imagga_scale,f_auto,fl_progressive,h_420,q_auto,w_1000/https://thepracticaldev.s3.amazonaws.com/i/dhrfe0ncjt2wt5u5mnfs.png)
#### Develop a program in python to take email and password as input and check send an automated message. 

![](/memes/meme.png)

[Disable this first in order to login through command line](https://myaccount.google.com/lesssecureapps?pli=1&rapt=AEjHL4PmynDZrUjYRUrNxY1kqLGsn1d_z-Q5A_fSFHq9KBMLcbgshEx3LqomD25BMuYeNC4ehMAg9OBHwsK32dsBizNBPsDqlA)




    import smtplib

    from getpass import getpass

    server = smtplib.SMTP_SSL("smtp.gmail.com", 465)


    email_id = input("enter your email: ")
    password = getpass()

    server.login(email_id, password)

    server.sendmail(email_id, "aakashcoder1210@gmail.com", "hello aaki")

    print("Email sent")
    server.quit()





![](/memes/end.jpg)




