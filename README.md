# dmsc-log
Devlog for Drawing, Moving and Seeing Code

## Class Notes
Notes from class 


5/6/21
Alright so I have clearly not touched this log since the first weeks of class and thats my fault. I missed half of the 2nd week becuase my house flooded and then becuase of that I was displaced and couldn't make it to class the following week. These early absents definitely set me behind and while trying to manage with other classes, my job, and my home life, I just struggled to find the time to catch up. My plan is to go through the assignments where I was to post on here and explain what I did at the time, becuse I was doing the coding for this class, I just completely fotgot to update this in the process.


## Squirell Group Project Log

This the devolg post for my work and experience working on the squirel project. I worked with Chris, Monty, and Quincy.  We first started out by
making a google drive file where we could post all of the planning and coding with each other. The first class we each took our own task and worked 
on them individually, but asked each other for help. While I wasn't to confident at coming up with the more complex probelms, I worked on getting player/
enemy movement. Chris and Quincy worked on how the squirells would eat one another and subsequently grow in size, while Monty worked on how the squirells 
would look. All of our code was in the google drive so each were running our own version of the game. This was about as far as we got and class and then 
we didn't meet up again until before the next class where Lee gave us time to work on it some more. Quincy had the most complete version of what we had 
worked on prior so we decided to use his as the main code. In the time before class we worked on some of the final things that we felt we could get done and 
Quincy finalized the code. 

here is the link to the code:

https://editor.p5js.org/quincywashington/sketches/8I4NXn2g8C




## FINAL PROJECT LOG


In the begining of the semsester we talked a lot about emergence and interactive enviorments and my project for that was to create a duck pond that would have bread that they could eat. One of my favorite games is untitled goose game, where you get to run around do fun things as a goose. I loved the artstyle and the basic premise of the game so I felt like making my own (much less cool) version of it. We also needed to have procedural generation so I felt that the map was the easiest to impliment for that task. My game is based on the grid generation that we went over in class and has 5 levels of increasing dificulty. (pictured below)

![Screen Shot 2021-05-16 at 7.42.33 PM.png]({{site.baseurl}}/Screen Shot 2021-05-16 at 7.42.33 PM.png)
![Screen Shot 2021-05-16 at 8.00.33 PM.png]({{site.baseurl}}/Screen Shot 2021-05-16 at 8.00.33 PM.png)
![Screen Shot 2021-05-16 at 7.43.34 PM.png]({{site.baseurl}}/Screen Shot 2021-05-16 at 7.43.34 PM.png)
![Screen Shot 2021-05-16 at 7.43.13 PM.png]({{site.baseurl}}/Screen Shot 2021-05-16 at 7.43.13 PM.png)
![Screen Shot 2021-05-16 at 7.42.48 PM.png]({{site.baseurl}}/Screen Shot 2021-05-16 at 7.42.48 PM.png)


Once I got the generation to work, I worked on aesthetics for a little bit. I changed the background to blue for the water, and then had 8-bit lily pads spawn in the location the blocks were spawning in. I ran into a little trouble here because I wasn't sure where to impliment it, but after a few trial and errors, I figured it out. 
![Screen Shot 2021-05-16 at 7.40.04 PM.png]({{site.baseurl}}/Screen Shot 2021-05-16 at 7.40.04 PM.png)
After this I got an image of a duck that I could use and just replaced the ball I was originally working with and it was time to impliment the bread. Becuase I wanted 5 to spawn, I started by making an array and a variable that would determine the max amount. I also relized that I wanted them to spawn essentially the same way as the duck, so all I had to do was take the players code and duplicate it. I got them spawning in random locations and then went to work on the hit boxes. When I originally wrote the code, I felt that having vectors for the positioning was the easiest way to do hit-boxes. However this proved to be the biggest challenge and it took me a long time and a phone-a-friend to figure out how to do it. You can see the code below.
![Screen Shot 2021-05-16 at 7.41.17 PM.png]({{site.baseurl}}/Screen Shot 2021-05-16 at 7.41.17 PM.png)
After I got the hit boxes to work properl, it was time to add the game mechanics of "eating" and the progression of levels. I made a basic variable to set the score to 0 when the game starts and when the duck interacted with the bread, it would add one. Also so it didn't just add a bunch, I needed the bread to despawn. After a couple failed attempts at trying to impliment the splice function, I decided it would just be easier to have them move their location far off screen. I also needed to figure out how I would do the progression of levels. I had a new level added for every 5 pieces of bread eaten (the amount that spawned) and had the sketch reset when that number was met. I also made it so that in the map generation code, the rate at which the spawining of lily pads would increase. This can be seen in the code below. 


