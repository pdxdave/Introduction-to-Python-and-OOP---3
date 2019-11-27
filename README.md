# Introduction-to-Python-and-OOP---3
Introduction-to-Python-and-OOP---3

```
class Store:
    def __init__(self, name): #constructor
        self.name = name

    def __str__(self): # called to print name of obj as a string
        return f"store: {self.name}"
    
    def __repr__(self):
        # think of this as being used for debugging
        return f'Store: ("' + self.name + '")'
    

my_store = Store("Dave's") # new store object
```
