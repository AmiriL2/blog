# Class ToDo Project: How To Do and How It Was Done

### **What Was Done**
Recently, we created a Todo list in class. The abilities the ToDo list has to have is to allow the user to add and remove things from the list, as well as tell you what your current ToDos are.

### **How To Create**

The first step of a todo list is allowing it to repeat itself after you complete whatever you wanted to say. So what do you use for this? A while loop! If you use a while loop and set the condition to true 
```python
while True:
```
 , everthing under the while toop will repeat after you finish entering what you want to enter into the list.

### **Inputs**

In order to get what the user wants to do, you have to use an input
```python
todoinput = input("Would you like to add or remove a todo?")
```

Another input that you have to use is to ask what do they want to add and also what do they want to remove.
Ex.

1) ```python
    REMOVE = input("what would you like to remove? ")
    ```

2) 
    ```python
    ADD = input("what is your new todo? ")
    ```

You must set them as equal to something for a reason that will be spoken on later on


In total this is what I did:

```python
ToDo = ["get cash", "spend cash", "cry"]

while True:

   
    print("")
    todoinput = input("Would you like to add or remove a todo?")
    print("")
    if todoinput == ("add"):

        ADD = input("what is your new todo? ")

        
        ToDo.append(ADD)

    elif todoinput == ("remove"):

        REMOVE = input("what would you like to remove? ")
        print("")
        
        if REMOVE in ToDo:
        
            ToDo.remove(REMOVE)
        
        else:
            print("Error: This is not in the list")
            print("")

    else: 
        print("Incorrect Input")
        print("")
        print("")
    print("~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~")
    print("")

    print("Your current todos are: " )
    X = 1 

    for T in ToDo:

        print(str(X) + ") " + T)

        X +=1

```