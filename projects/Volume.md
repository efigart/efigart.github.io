---
layout: project
type: project
image: img/cube.jpg
title: "Area and Volume Calculator"
date: 2023
published: true
labels:
  - C
summary: "This program calculates the Area and Volume of an object. It was an assignment for ICS 212."
---

This program was made for an assignemnt in ICS 212. It was written in C and models class hierarchy and polymorphism. The user is instructred to select a number from 1 - 7 that correspondes to an array filled with various shape objects. If the input is valid, the user is then instructed to input the measurments of their desired shape. The information is then passed to a designated class that calculates and returns the volume and area of the shape. The main method implements a while-loop, this means the user can continue to run calculations until they choose to exit.

This program showcases class heirarchy. For example, the object Cube is a subclass of the Square object. Additionally, Square object is a subclass of the Shape object. Writing this program was very repetive, each shape had it's own class and was filled with 4 or 5 methods. It wasn;t very difficult, but it was very time consuming. Despite this, it really allowed me to understand inheritance. 

Here is some code showing the Shape object:

```cpp
class Shape {
public:
  /** Returns the name of the class. */
  virtual const char* name() const = 0;
  /** Prints the area or surface area, and volume of the object. */
  virtual void printDetails() const = 0;
  /**                                                                                                                                                       
   * Prompts the user to enter a radius, side, and/or height                                                                                                
   * of the object and set the appropriate data member(s).                                                                                                  
   */
  virtual void inputData() = 0;
  /** Calculates and returns the area or surface area of the object. */
  virtual double area() const = 0;
  /** Calculates and returns the volume of the object. */
  virtual double volume() const {
    return 0.0;
  }
};

```




