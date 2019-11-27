# Introduction-to-Python-and-OOP---3
Introduction-to-Python-and-OOP---3

```
class Dept:
    def __init__(self, name): #constructor
        self.name = name

    def __str__(self): # called to print name of obj as a string
        return f"dept: {self.name}"
    
    def __repr__(self):
        # think of this as being used for debugging
        return f'Dept: ("' + self.name + '")'


class Store:
    def __init__(self, name, depts): #constructor
        self.name = name
        self.depts = depts

    def __str__(self): # called to print name of obj as a string
        return f"store: {self.name}"
    
    def __repr__(self):
        # think of this as being used for debugging
        return f'Store: ("' + self.name + '")'
    

depts = [
    Dept("Department1"),
    Dept("Department2"),
    Dept("Department3"),
]



my_store = Store("Dave's", depts) # new store object
print(my_store)

dept1 = Dept("Department1")
print(dept1)
```
