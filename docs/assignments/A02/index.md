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
   -_Angles and Reactions_
        <img width="3401" height="2279" alt="IMG_3342" src="https://github.com/user-attachments/assets/63b1994d-7d33-42c6-bab6-a92b63f24556" />

First off in the calculations I had to determine the angle that my triangles had so that way I could do my internal load calculations properly. For my middle triangle I split it in half which gave a base of 0.2 m and a height of 0.3 m, I then had to take arctan (0.3 m/0.2 m), as this is the required formula to obtain an angle for triangles, this in turn gave me an angle of 56.31 degrees in the bottom left of the triangle. For the inverted triangle I did roughly the same thing, however I had to cut 0.4 m away from roller B so that way it would end up as a right triangle. Know that it was cut properly I took arctan (0.3 m/0.4 m) and obtained 36.86 degrees in the upper left corner of the triangle. Now that I had the angles all I needed was the reactions at B and A so I could begin finding internal loads in all my members. So, to obtain the reaction at A I had to take a moment about roller B; MB=0= (0.04 m)(3)(Ay)+20 kN(0.4 m)-20 kN(0.8 m), this in turn gave me a reaction of roughly 6.67 kN=Ay. Now since all loads were applied in the y-direction I can assume that Ax=0 since nothing pushes or pulls in that direction. Now that I have my first reaction I can easily obtain my second by taking a sum of all forces in the y-direction; Fy=0=By+6.67 kN+20 kN-20 kN, this in turn gave me a reaction of -6.67 kN=By. Now that I had the angles and reactions at both A and B I could finally start solving for my internal loads in all my truss members.

   -_Internal Loads_

<img width="3024" height="3203" alt="IMG_3346" src="https://github.com/user-attachments/assets/495bf4e0-7ddb-47cf-a8e2-01730ec9cdaa" />

To begin calculating my internal loads I had to choose a spot that would statically determinate, so I choose joint B as it had one known and two unknowns which makes it possible to solve for the internal loads as it is statically determinate there. I took a sum of all the forces in the y-direction to start; Fy=0=-By-BC sin(36.86), which rearranged to solve for joint BC becomes; BC=-BY/sin(36.86), I plugged in my numbers and got BC=11.12 kN in compression. So now that joint BC was solved, I could find joint BE by taking a sum of all forces in the x-direction; Fx=0=BE+BC cos(36.86), which rearranged to solve for BE becomes; BE=-BC cos(36.86), putting the numbers in gave BE=8.897 kN in tension.

<img width="3024" height="4032" alt="IMG_3345" src="https://github.com/user-attachments/assets/20cec03d-05eb-4787-9b8d-242145100df7" />

Now that I solved joint B I could move onto joint C to find the final internal loads of the truss due to it being symmetric. So, to start things off I took a sum of all forces in the y-direction again; Fy=0=CE sin(56.31)-BC sin(36.86)+P, when I rearranged this one to solve for CE it came out like this; CE=-(P+BC sin(36.86)/sin(56.31), and after I put the numbers in it gave me CE=16.02 kN in compression. Now that I have joint CE solved, I could now take a sum of the forces in the x-direction to find CD;
