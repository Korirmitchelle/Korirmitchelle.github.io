---
layout: post
title: You're up and running!
---


Object-oriented programming (OOP) is a programming language model organized around objects rather than "actions" and data rather than logic. Historically, a program has been viewed as a logical procedure that takes input data, processes it, and produces output data.

OOP makes your programs more flexible and understandable.

## PROCEDURAL VS OOP


Procedure Oriented Programming| Object Oriented Programming 
---                          | ---
In POP, program is divided into small parts called functions. | In OOP, program is divided into parts called objects      
  |
POP does not have any access specifier.  | 	OOP has access specifiers named Public, Private, Protected, etc.
    |   
In POP, Data can move freely from function to function in the system. |	In OOP, objects can move and communicate with each other through member functions.
    |       



## INHERITANCE

Inheritance can be defined as the process where one class acquires the properties (methods and fields) of another. With the use of inheritance the information is made manageable in a hierarchical order.

The class which inherits the properties of other is known as **subclass** (derived class, child class) and the class whose properties are inherited is known as **superclass** (base class, parent class).

### Why Inheritance Is Good

* Decreases duplicate code

- Eliminates looking for what code needs to be changed

+ Avoids breaking previously working code 

## POLYMORPHISM

 **Polymorphism** can be achieved through overriding. Put in short words, polymorphism refers to the ability of an object to provide different behaviors (use different implementations) depending on its own nature. Specifically, depending on its position in the class hierarchy.

**Method Overriding** is when a method defined in a superclass or interface is re-defined by one of its subclasses, thus modifying/replacing the behavior the superclass provides. The decision to call an implementation or another is dynamically taken at runtime, depending on the object the operation is called from. Notice the signature of the method remains the same when overriding.

**Method Overloading** is unrelated to polymorphism. It refers to defining different forms of a method (usually by receiving different parameter number or types). It can be seen as static polymorphism. The decision to call an implementation or another is taken at coding time. Notice in this case the signature of the method must change.

## INTERFACES

An interface is a shell that provides the names of all the variables and methods but no code.

You describe what other classes will do with it but don't describe exactly how; hence polymorphism can be used without all of the problems.
