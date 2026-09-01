# A2 – Truss Stress Analysis

## **Objective**
-Design a lightweight planar truss using A500 steel or an alternative material.

-Create free body diagrams (FBDs) for joints and critical pins.

-Calculate the required cross-sectional area of truss elements with a safety factor.

-Determine pin sizes based on shear forces with a safety factor.

-Solve equations symbolically and numerically for both truss and pin design.

-Estimate the total weight of the truss and pins.

-Create a CAD model with accurate dimensions and connections.

-Compare CAD weight predictions with hand calculations.

-Document key engineering lessons learned from the process.

## **Deciding**

<img width="3089" height="2039" alt="IMG_3341" src="https://github.com/user-attachments/assets/57d82db8-fa5f-4e7e-975b-31165d512855" />

I decided to go with the most basic geometric design for my truss, triangles, as I wanted to keep it relatively simple, easy to work on, and have the truss be able to hold structural integrity while under load. I also gave the truss a 20 kN load which decreased my reaction and internal loads upon the truss I designed. The two inverted triangles have a base of 0.6 m with a height of 0.3 m; on the other hand, the center triangle has a 0.4 m base and a 0.3-meter height. This makes the overall truss have a length of 1.2 m and a height of 0.3 m. I also had to implement five pins due to the roller/fixed pin connections and where the loads were applied as well, and I also needed one extra pin for joint E so that way my whole truss could be held together tightly. This way with truss geometry and five pin setup my truss could easily handle any stress that would be applied by the 20 kN loads that I chose. Since the truss is completely symetric down the middle anything that happens on one side will be the opposite on the other since one load pushes up and the other down.

## **Calculations**
   -Angles and Reactions
        <img width="3401" height="2279" alt="IMG_3342" src="https://github.com/user-attachments/assets/63b1994d-7d33-42c6-bab6-a92b63f24556" />

First off in the calculations I had to determine the angle that my triangles had so that way I could do my internal load calculations properly. For my middle triangle I split it in half which gave a base of 0.2 m and a height of 0.3 m, I then had to take arctan (0.3 m/0.2 m), as this is the required formula to obtain an angle for triangles, this in turn gave me an angle of 56.31 degrees in the bottom left of the triangle. For the inverted triangle I did roughly the same thing, however I had to cut 0.4 m away from roller B so that way it would end up as a right triangle. Know that it was cut properly I took arctan (0.3 m/0.4 m) and obtained 36.86 degrees in the upper left corner of the triangle. Now that I had the angles all I needed was the reactions at B and A so I could begin finding internal loads in all my members
