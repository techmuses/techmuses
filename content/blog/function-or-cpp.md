---
title: "What is Function Overiding Problem in C++ and how to Solve?"
date: 2018-11-07T11:40:11+02:00
publishdate: 2018-11-07T11:40:11+02:00
image: "/images/blog/overide.gif"
tags: ["coding", "cpp"]
comments: false
ReadingTime: "6"
AuthorName: "Jainal"
Description: "The Conjuror"
Thumbnail: "/images/jainal.jpg"
Summary: "First Let Us Understand what is function overriding problem.Inheritance in C++ Inheritance allows software developers to derive a new class from the existing class. The derived class inherits features of the base class (existing class)."
---

## First Let Us Understand what is function overriding problem!

**Inheritance** in C++ Inheritance allows software developers to derive a new class from the existing class. The derived class inherits features of the base class (existing class).

C++ allows you to specify more than one definition for a **function** name or an **operator** in the same scope, which is called **function overloading** and **operator overloading**respectively.

An overloaded declaration is a declaration that is declared with the same name as a previously declared declaration in the same scope, except that both declarations have different arguments and obviously different definition (implementation).

This Causes Chaos and Confusion !!


## Lets Get a Wide Perspective By Seeing this 
`Code of Function Overiding`

**This Is a Typical Function Overriding Program:-**

![enter image description here](https://cdn.programiz.com/sites/tutorial2program/files/function-overriding-C++.jpg)

 - As u can see when we call the above function the compiler will get
   confused as to which function to call.
  
 - See sum value in output . 
 - `****sum=4354132****   <-------  This Is a Random Garbage Value. 


So How Do i Solve it???  

![enter image description here](https://img.buzzfeed.com/buzzfeed-static/static/2015-11/3/14/enhanced/webdr05/anigif_enhanced-26180-1446577790-7.gif)

*Dont Worry Sailor i Got Your Back Covered!!*

 - [x] Here is How you Do It

**Observe This Code:-** 
![enter image description here](https://cdn.programiz.com/sites/tutorial2program/files/access-member-function-base-class-C++.jpg)

Got A Eureka Sensation!!

![enter image description here](https://steemitimages.com/0x0/https://media.collegetimes.com/uploads/2014/04/cxXlF3X.gif)

## *Its That easy!!*

**`Here is a Program to Keep U started`**

   

     #include <iostream>
    
    using namespace std;
    
    class Base
    
    {
    
    public:
    
    int a,b;
    
    void getData(){
    
    cout<<"Enter values of a & b:";
    
    cin>>a>>b;
    
    }
    
    };
    
    class Derived:public Base
    
    {
    
    public:
    
    int sum;
    
    void getData(){
    
    Base::getData();
    
    sum=a+b;
    
    cout<<endl<<"sum="<<sum;
    
    }
    
    };
    
    int main()
    
    {
    
    Derived obj;
    
    obj.getData();
    
    }

******************************************************
   **Enter values of a & b:
   10
   20
   sum=30**
******************************************************