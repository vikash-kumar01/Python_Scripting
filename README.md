## PYTHON SCRIPTING
      
      import sys
      print(sys.version)    # Prints Installed python Version
      
## OS MODULE
    
    import os

    print(os.getcwd())   # Shows PWD

    print(os.chdir("/etc/ansible/hosts"))   # Change Directory (// or / backslash both works here..)

    print(os.mkdir("/home/repl/testdir"))   # Create Directory

    os.rmdir("/home/repl/testdir")         # Removes a Directory

    os.remove("/home/repl/testdir/demo.txt")  # Removes the file

    os.path.join("D:\\home\\repl\\testdir","D:\\home\\repl\\testdir\\demo.txt")  # Joins the path (o/p /home/repl/testdir/demo.txt)
    
    os.path.split("D:\\home\\repl\\testdir")  #Splits the path and File (O/p : D:\\home\\repl\\testdir "demo")

    print(os.path.exists("D:\\home\\repl\\testdir")) # Return True/ False if path Exists
    
    
## SUBPROCESS MODULE

    Module Let's you interact with OS + Create New Processes + Pass Info Into or Out Of it + get return Codes


## MATH MODULE
   
    import math

    print(math.pi)
    print(math.e)
    print(math.degrees(0.1))
    print(math.asin(0.5))   # a because we want values in radian
    print(math.acos(0.5))
    print(math.exp(2))
    print(math.log(10,10))  #log10 base 10
    
    
# RANDOM MODULE

    Used to generate Random numbers 
    
    
    import random

    print(random.randrange(50))        # Print Random number <=50
    print(random.randrange(10,50))     # Print random number between a range
    print(random.randrange(10,50,10))  # Print random number between a range and step size of 10 ( 10,20,20)
    print(random.randint(0,20))        # print random int number between a range 


## DATETIME MODULE

    import datetime

    print(datetime.date.today())  # Displays the Current date

    # ARITHEMETIC FUNCTION OF DATETIME OBJECT (Attributes are Days, seconds and microseconds)
    now = datetime.datetime.today()
    other = datetime.datetime(1994,10,10,17,59)
    print(now-other)


## JSON MODULE

    Popular in Communicating between Web Servers and Clients + Converts python objects to serialize representations(JSON OBJECTS) 
    
    
    
    import json
    Employees_data= '''
    {
    "Employees" : [
     {
    "userId":"rirani",
    "jobTitleName":"Developer",
    "firstName":"Romin",
    "lastName":"Irani",
    "preferredFullName":"Romin Irani",
     "employeeCode":"E1",
     "region":"CA",
     "phoneNumber":"408-1234567",
     "emailAddress":"romin.k.irani@gmail.com"
     }
    ]
    }
    '''
    print(Employees_data)

    #Conversion 
    data= json.loads(Employees_data)
    print(data)
