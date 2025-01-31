---
layout: project
type: project
image: img/note.png
title: "Playlist Mdoel"
date: 2022
published: true
labels:
  - Java
summary: "A program to model a playlist. This was an assignment for ICS 111."
---

This program was made for an assignemnt in ICS 111. It was written in Java. It
models a playlist using objects and an array list. It promopts the user to enter 
a song name, artist, minutes, and seconds. These values are passed to a constructor for a song 
object. If all of the values are valid, an object is created and then stored in an array list. 

The program utilizes a while-loop to allow the user run the program for as long as they like.
It displays a menu that lists options 1 - 4. These include adding a song, removing a song, 
viewing the full playlist, and exiting the program. In case of an invalid input, I utilized 
an exception to display an error message and return the user to the menu. 

This project was made duirng my first ICS class and allowed me to incoroprate many 
different aspects of coding into one project. It deepend my knowledge and understanding
of objects and array lists. It also helepd me learn more about custom exceptions. Writing the 
code was very repetitive, but it helped me remeber the format and outline for creating objects
with differnt methods. 

Here is some code of the song object constructor

```cpp
/**
    * constructs song object 
    *
    * @param         title                title of song  
    * @param         artist               artist of song
    * @param         minute               minutes in song  
    * @param         second               seconds in song 
    *
    * @exception     SongException        if the title is not at least 2 characters  
    * @exception     SongException        if the artist is not at least 2 characters 
    * @exception     SongException        if the minutes is not between 1 - 99
    * @exception     SongException        if the seconds is not between 0 - 59 
    */
   
   public Song() {
   
   }
   
   public Song(String title, String artist, int minute, int second) throws SongException {
      
      this.setTitle(title);
      
      this.setArtist(artist);
      
      this.setMinute(minute);
      
      this.setSecond(second);
      
   }
```


