---
layout: essay
type: essay
title: "Final Project Idea"
date: 2025-04-01
labels:
  - Software Engineering
  - Nextjs
---

## Overview

### Problem

Parking at Zone-20 can sometimes be challenging. After a certain time, especially on certain days (Tuesday, Wednesday, Thursday), finding an open spot can be very difficult. This primarily impacts students who have classes later in the day. 

### Solution

This idea is built / expanded off the parking-reservation project that was mentioned during class. InsertName is an application that allows students to track availiable spots in Zone-20.

- when students arrive (presumably in the morning) they can input their stall number / location into the app
- when they leave, they can open the app and mark their spot as available
- students arriving later in the day (when the lot is relatively full) can open the app and view a list of available spots, eliminting the need to endlessly circle the lot
- if they take a spot listed on the app, they can mark it as taken and it will be removed from the list of available spots

## Approach

To preface, this application would be voulantary. I don't think it would be realistic to expect everyone who parks in Zone-20 to particpate. Also, in order for this to work, there would have to be some sort of numbering / identification system for the stalls.

Although non-students also utilize the lot, the main purpose of this app would be to assist students. So this application would only be accessible with an account created with a UH email.

This appliction would have two user groups: Students and Admin. Students can veiw / add / remove spots. Admins have access to the full site + data. 

Some possible mockup pages include:

- landing page
- view avilable spots
- add spot
- remove spot
- admin home page

## Use Case Ideas

- a new user arrves at the landing page and is prompted to make an account
- a user opens the "add spot" page, and inputs their stall number / location
- later, the same user opens the "remove spot" page and marks their spot as avialable
- the stall number is then passed and displayed on the "view available spots" page
- a different user arrives (when it is crowded), logs in / creates an account, and opens the "view available spots" page
- they pick from the list of spots and drive to it, if it is available, they park, open the "add spot" page, and input their stall number / location
- the stall is removed from the "view avilable spots page"

## Beyond the Basics 

- the "view available spots" page is sorted by time
- a spot will be automatically removed from the "view available spots" page after a pre-determined amount of time 
- admins can view inputs from the "add spot" page 
- a student is only allowed to "add" one spot at a time
- a student can only "remove" a spot they have previously added
 

