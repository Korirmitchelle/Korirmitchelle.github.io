---
layout: post
title: Getters and Setters
---


**Mutator** method is a method used to control changes to a variable. They are also widely known as **setter methods.** Often a setter is accompanied by a **getter** (also known as an accessor), which returns the value of the private member variable.

The mutator method is most often used in object-oriented programming, in keeping with the principle of **encapsulation.** According to this principle, member variables of a class are made private to hide and protect them from other code, and can only be modified by a public member function (the mutator method), which takes the desired new value as a parameter, optionally validates it, and modifies the private member variable.

Mutator methods may also be used in non-object-oriented environments. In this case, a reference to the variable to be modified is passed to the mutator, along with the new value. In this scenario, the compiler cannot restrict code from bypassing the mutator method and changing the variable directly. The onus falls to the developers to ensure the variable is only modified through the mutator method and not modified directly.

In programming languages that support them, properties offer a convenient alternative without giving up the utility of encapsulation.


In Java getters and setters are completely ordinary functions. The only thing that makes them getters or setters is convention. A getter for foo is called getFoo and the setter is called setFoo. In the case of a boolean, the getter is called isFoo. They also must have a specific declaration as shown in this example of a getter and setter for 'name':


   class Today
   {
    private String name;

    public Today() {}

    public Today(String name) {
        this.name = name;
    }

    public String getName() {
        return this.name;
    }

    public void setName(String name) {
        this.name = name;
    }
}


The reason for using getters and setters instead of making your members public is that it makes it possible to change the implementation without changing the interface. Also, many tools and toolkits that use reflection to examine objects only accept objects that have getters and setters. JavaBeans for example must have getters and setters as well as some other requirements.