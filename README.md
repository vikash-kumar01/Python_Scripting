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

   # Module Le's you interact with OS 

