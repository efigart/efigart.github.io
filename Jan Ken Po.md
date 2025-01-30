---
layout: project
type: project
image: img/JanKen.png
title: "Jan Ken Po Emulator"
date: 2023
published: true
labels:
  - Java
summary: "Assignment for ICS 211."
---

This program was made for an assignemnt in ICS 211. It was written in Java and implements multiples classes, and a GUI (Graphic USer Intereface). 

It allows the user to select rock, paper, or scissors through buttons, while hthe computer randomly chooses an option. ASCII art is used to 
visually represent both choices. The winner of each round and the current score is displayed on the interface. 

The user is allowed to end the game at any time by pressing an "exit" button. When this happens, the score is saved to a txt file named "scores.txt". 

Here is some code that shows the initilization proecss for some elemets of the GUI.

```cpp

   private JButton rock = new JButton("Rock");   
   
   private JButton paper = new JButton("Paper");
   
   private JButton scissors = new JButton("Scissors");
   
   private JButton in = new JButton("Instructions");
   
   private JButton exit = new JButton("Exit");
   
```
Here is some code that shows the ACSII art implementation

```cpp

userDraw.setText("<html>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;_______<br>" +
                             "---'&nbsp;&nbsp;&nbsp;&nbsp; ____) <br>" +
                             "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(_____) <br>" +
                             "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(_____) <br>" +
                             "&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;(____) <br>" +
                             "---.__(___)<br>" +
                             "</html>");

```        
