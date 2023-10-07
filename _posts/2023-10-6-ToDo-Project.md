# ToDo Project: How To Create

### **What Was Done**
Recently in FSD, we created a Todo list using python. The abilities the ToDo list has to have is to allow the user to add and remove things from the list, as well as tell you what your current ToDos are.

### **How To Create**

The first step of a todo list is creating the list itself, so for what we will do, we will create a list and mark the name as ToDo. 

Example:
```python
     ToDo = ["get cash", "spend cash", "cry"]
```

Allowing it to repeat itself after you complete whatever you wanted to say. So what do you use for this? A while loop! If you use a while loop and set the condition to true, everthing under the while toop will repeat after you finish entering what you want to enter into the list.
```python
while True:
```

### **Inputs & If Statements**

In order to get what the user wants to do, you have to use an input. The input we will use is asking the user would they like to add or remove something from the list. An exampke of what we will use is posted here:

```python
    todoinput = input("Would you like to add or remove a todo?")
```

Another input that you have to use is to ask what do they want to add and also what do they want to remove. For these inputs though, inputs you must set these inputs as equal to something. This is because you have to remove or add the input to the list depending on what the user types in

You must also put these inside of if and elif statements because if the users input is "add", then we will use the .append the item to the list. If the user types in "remove" then we will use the .remove feature to remove item from the list. For the remove part we want to also use an else statement .This is because if they item is not in the list it cannot be removed, so we will print out that an error has occured and that the item cannot be listed. Here is an example of this:

```python
    if todoinput == ("add"):

        ADD = input("what is your new todo? ")

        ToDo.append(ADD)

    elif todoinput == ("remove"):

            REMOVE = input("what would you like to remove? ")
            
            if REMOVE in ToDo:
            
                ToDo.remove(REMOVE)
            else:
                print("Error: This is not in the list")
```

If neither of these is what the user has inputed, then the code should return an error saying that the input that we were looking for was not found/was not inputed by the user. We will do this by using an else saying that if all else was not inputed, then print "Incorrect Input"

```python
    else: 
            print("Incorrect Input")
```
### **Finishing Touches**

In order to allow the code to print out the todos, you must use a for loop. This for loop must say that for T in todos, print out the todos. This T will represenent the values inside of the list. However, that is not all that we will be doing. We will be also printing out the number of todos next to the todos in the list. 

The way we will do this is by setting a value to one. In this example, we will use X. Everytime we add another item to the todo, the number will go up. We do not have to worry about the remove because when you remove an item from the list the number in the list will go down by one. 

Although, putting these all together will not print out properly and result in a syntax error. Why might you ask? Because X is printed out as an integer, not a string. So what you must do is convert X back to a string by doing str(X). After doing that, now you may put these altogether and have a proper printout.

```python
    print("Your current todos are: " )

    X = 1 

    for T in ToDo:

        print(str(X) + ") " + T)

        X +=1
```
### **Extras**

Now, if you want your code to print out more spaced out and easier to read, I would recommend putting empty print("") statements throughout the code. I would also suggest that you create a print out a bunch of tildes inside of a print statement directly below the "Incorrect Input" that was printed out listed above. 

```python
print("~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~")
```

That way when you use the code it should print out like any of these depending on what option you choose:

1) 
![Example of how the code should print out](/assets/example.png)

2)
![Second example of how the code should print out](/assets/example2.png)

3)
![third example of how the code should print out](/assets/example3.png)


