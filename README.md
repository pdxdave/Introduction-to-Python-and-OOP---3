# Introduction-to-Python-and-OOP---3
Introduction-to-Python-and-OOP---3

```
class Dept:
    def __init__(self, name, num): #constructor
        self.name = name
        self.num = num

    def __str__(self): # called to print name of obj as a string
        return f"dept: {self.num}: {self.name} "
    
    def __repr__(self):
        # think of this as being used for debugging
        return f'Dept: ("' + self.name + '")'


class Store:
    def __init__(self, name, depts): #constructor
        self.name = name
        self.depts = depts

    def __str__(self): # called to print name of obj as a string
        s = f"store: {self.name}\nDepartments:\n"
        
        for d in self.depts:
            s += f" {d.num} : {d.name}\n"
        
        return s
    
    def __repr__(self):
        # think of this as being used for debugging
        return f'Store: ("' + self.name + '")'
    

depts = [
    Dept("Department1", 11),
    Dept("Department2", 22),
    Dept("Department3", 33),
]



my_store = Store("Dave's", depts) # new store object
print(my_store)

# dept1 = Dept("Department1")
# print(dept1)
```
