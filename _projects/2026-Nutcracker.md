---
layout: project
title: Design your own Nutcracker 
description: How I created my own nutcracker
image: /assets/images/Diagram.jpg
---



PART 1:
Problem statement and objective: 
I needed to design a usable nutcracker given certain paramteres. 

Constraints and input paramters:
The needed force to crack the nut ~2220N and the average applied force ~500. The radius of the nut is 1 cm. 

My approach to the problem: 
My approach was to first take the moment about the pin at the nutcracker, which was the part furtheset away from the handle. 
Based on how I designed the nucracker, It allowed for the only part of the radius vector that I had to take into account, was
the part along the i^ axis. The radius until the nut I designated as x1, and the radius until the applied for I measure as x1+x2. 
Taking the moment about the pin would allow me to find these two values of x1 and x2 that would balance the forces sufficently. 
Once I found the lengths, I had the complete diagram of the nutcracker. 

Diagram of the Nutcracker:

![Diagram]({{ "/assets/images/Diagram.jpg" | relative_url }}){: .inline-image-l}


Discussion on usability of the design: 
This design was usable as you only needed to apply 500N of force on each end with a 1cm gap in between. 

PART 2: 
Problem statement and objective: 
Given the design of the nutcracker as stated above I now needed to: 
#1 Find the location of maximum elastic deflection in your handles. 
#2 Choose a “beam” design (cross-section, material) such that the vertical elastic deflection is below 2% of its length and is the most mass-efficient possible.
#3 Present the final diamgram as in an image or drawing.

Constraints, input paramaters, and assumptions: 
For this second part I kept the same applied force and force to crack the nut. The assumption that I made was that the bar was straight from the pin to the nut to the point of applied force. 

My approach to the problem: 
Given these assumptions the I used the following approaches: 
(a) I created a free body diagram, where there were only three fources that acted upon it. #1 the Applied force of 500N, #2 the reaction force from the nut and #3 the force at the pin. Because I have the lengths described as above, I was able to use the appendix within Statics and Mechanics of Materials (Ferdinand P. Beer) and modeled it such that Xm (the point of applied load) was position at ((L^2-a^2)/3)^1/2 where when pluggin in the known lengths for L and using a as 2cm as would be described in the model, I got that xm = 3.214 cm.
(b) I used the same appendix which allowed me to find the equation for the maximum deflection. Because the maximum deflection can only be two percent of the length I used: Ymax = L*0.02 = (Pa(L^2-a^2)^3/2)/(9Sqrt(3)EIL), thus to answer the question we need to find the cross section and the material. This depends on the two variables E and I, all else are givens. So I isolated for them and now needed to choose materials such that it was the most mass effective. Using the same appendix, I found that a optimal material would be structural steel as it is sturdy to not deform a lot while still not being incredibley heavy. In addition, using the E=200GPA for steel this when done out gives the best W beam per unit shape to be the W 18x106
(c) attatched is the diagram that I would use for this nutcracker. 

![Diagram]({{ "/assets/images/image-1.png" | relative_url }}){: .inline-image-l}


Assistence: I went to office hours, where they helped me understand the problem and how to approach it.
