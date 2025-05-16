---
layout: essay
type: essay
title: "The Blueprint"
# All dates must be YYYY-MM-DD format!
date: 2025-04-24
published: false
labels:
  - UX Design 
---

## Blueprint 

I think Design Patterns serve as architectual blueprints for software development. They aren't regid instructions, but flexible templates that help tackle common challenges with proven solutions. The term "blueprint" may make it seem like you are confined to building the same structure everytime, but in reality, it is actually the opposite. Design patterns provide a solid foundation, but allow for full creative freedom in implmentation. An example of this would be adding customization to a house during construtcion, each change is subject to guidlines, but can be tailored to anything. Instead of limiting creativity or workflow, design patterns allow for easy descion making, clean and maintainable code, and ensure that teh critical needs are met. This reslts in efficent software, giving both developers and users the best experience. 

## Utilization 

One of the design patterns I have used is the Factory Pattern. This is the process of returning the correct result based on context. For example, in the landing page of the final project, there is a button located on the center of the screen with the text "Get Started". If the user is not logged in, when clicked, this button redirects them to the log-in / sign-up page. If the user is already logged in, pressing the button sends them to the profile page. This is important because it improves the expirence of the user. 

The final project also utilizes the Singleton Pattern. We use "useSession()" to provide a single shared user session through the app. There is only one "session" per user, and all componenets that call "useSession()" refer to the same instance. 


