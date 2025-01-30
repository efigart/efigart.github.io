---
layout: project
type: project
image: img/micromouse/micromouse-square.jpg
title: "Jan Ken Po Emulator"
date: 2022
published: true
labels:
  - C
summary: "Assignment for ICS 211."
---

This program was made for an assignemnt in ICS 211. It was written in Java and implements multiples classes, and a GUI (Graphic USer Intereface). 
It allows the user to select rock, paper, or scissors through buttons, while hthe computer randomly chooses an option. ASCII art is used to 
visually represent both choices. The winner of each round and the current score is displayed on the interface. The user is allowed to end the 
game at any time by pressing an "exit" button. When this happens, the score is saved to a txt file named "scores.txt". 

Here is some code that shows the initilization proecss for some elemets of the GUI.

```cpp
byte ADCRead(byte ch)
// declare buttons + labels + variables
   private JButton rock = new JButton("Rock");   
   
   private JButton paper = new JButton("Paper");
   
   private JButton scissors = new JButton("Scissors");
   
   private JButton in = new JButton("Instructions");
   
   private JButton exit = new JButton("Exit");
   
   private JLabel title = new JLabel("Jan Ken Po", SwingConstants.CENTER);

```
