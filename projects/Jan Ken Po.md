---
layout: project
type: project
image: img/JanKen.png
title: "Jan Ken Po Emulator"
date: 2023
published: true
labels:
  - Java
summary: "A program to emulate a rock paper sciccors game with a CPU. This was an assignment for ICS 211."
---

This program was made for an assignemnt in ICS 211. It was written in Java and implements multiple classes, a driver class, and a GUI (Graphic User Intereface). When the program runs, a seperate window opens. The program allows the user to select rock, paper, or scissors through buttons, while the computer chooses an option though a random number generator. When the user selects an option, ASCII art is used to display the choice. Additionally, the same is true for the CPU choice. The winner of the round is displayed and one point is added to the score board at the top of the screen. The game runs indefinety utilizng a loop. The user is allowed to end the game at any time by pressing an "exit" button in the GUI. When this happens, a thank you message is displayed and the scores are saved to a txt file.

This project was the culmination of many differnt subjects we had covered over the semester. Designing the GUI was a challenge, it incorporated lots of code that we had not used before. I remeber it took two horus for me to settle with a design and make sure it eveyrthing lined up right. The hardest part of this projectw as the ASCII art. It took a while for me to source designs for each of the hand signs. The real challenge was flipping them 180 degrees to display for the CPU. It took a lot of trial and error to get it to look correct. Additionally, the ASCII art was in html, which is something I hadn't used before, which made it more complicated. Overall it was a fun project. 


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
