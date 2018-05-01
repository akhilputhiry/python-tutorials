# Method Resolution Order (MRO)

Before saying about MRO I would like to introduce you to the `diamond` problem of multiple inheritance.

# Multiple Inheritance

I am not planning to reinvent the wheel. Read about it in [wikipedia](https://en.wikipedia.org/wiki/Multiple_inheritance)

# Diamond Problem

You have 4 classes `A`, `B`, `C`, `D`. Among these classes, `B` and `C` are inherited from `A` and class `D` is inherited from `B` and `C`

```
class A(object):
    pass
    
class B(A):
    pass
    
class C(A):
    pass

class D(B, C):
    pass
```
