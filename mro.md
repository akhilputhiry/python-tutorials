# Method Resolution Order (MRO)

Before saying about MRO I would like to introduce you to the `diamond` problem of multiple inheritance.

# Multiple Inheritance

I am not planning to reinvent the wheel. Read about it in [wikipedia](https://en.wikipedia.org/wiki/Multiple_inheritance)

# Diamond Problem

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
