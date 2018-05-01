# Method Resolution Order (MRO)

Before saying about MRO I would like to introduce you to `the diamond problem` of `multiple inheritance`.

# Multiple Inheritance

Read about it in [wikipedia](https://en.wikipedia.org/wiki/Multiple_inheritance)

# The Diamond Problem

You have 4 classes `A`, `B`, `C`, `D`. Among these classes, `B` and `C` are inherited from `A` and class `D` is inherited from `B` and `C`

```
class A(object):
    
    def display(self):
        print('Iron Man')
    
class B(A):
    
    def display(self):
        print('Hulk')
    
class C(A):
    
    def display(self):
        print('Thor')

class D(B, C):
    
    def display(self):
        print('Captain America')
```

What will be the output if someone tries to execute the `display` method of class `D`? Will it execute the `display` defined in class `B` or class `C`. This `confusion or ambiguity` is called the `diamond problem` and solution for this ambiguity is called the `Method resolution order (MRO)`

# Method Resolution Order (MRO)

When the above probem occurs, the Python interpreter does the following

* Look if method exists in instance class
* If not, looks if it exists in its first parent, then in the parent of the parent and so on
* If not, it looks if current class inherits from others classes up to the current instance others parents

So in our example the lookup path will be

* Look in `D`
* If not found, look in `B`
* If not found, look in `B's` first parent `A`
* If not found, going back in `B` other parent `None`
* If not found, look in `D` other parent `C`
