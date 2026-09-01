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

I decided to go with the most basic geometric design for my truss, triangles, as I wanted to keep it relatively simple, easy to work on, and have the truss be able to hold structural integrity while under load. Choosing something like squares, rectangles, or circles would make it hard to calculate and make the truss susceptible to breaking under intense loads. I decided to give the truss a 20 kN load applied at joint C and D which decreased my reaction and internal loads upon the truss I designed. The two inverted triangles have a base of 0.6 m with a height of 0.3 m; on the other hand, the center triangle has a 0.4 m base and a 0.3-meter height. This makes the overall truss have a length of 1.2 m and a height of 0.3 m. I also had to implement five pins due to the roller/fixed pin connections and where the loads were applied as well, and I also needed one extra pin for joint E so that way my whole truss could be held together tightly. This way with truss geometry and five pin setup my truss could easily handle any stress that would be applied by the 20 kN loads that I chose. Since the truss is completely symetric down the middle anything that happens on one side will be the opposite on the other since one load pushes up and the other down.

## **Calculations**
   -_Angles and Reactions_
        <img width="3401" height="2279" alt="IMG_3342" src="https://github.com/user-attachments/assets/63b1994d-7d33-42c6-bab6-a92b63f24556" />

First off in the calculations I had to determine the angle that my triangles had so that way I could do my internal load calculations properly. For my middle triangle I split it in half which gave a base of 0.2 m and a height of 0.3 m, I then had to take arctan (0.3 m/0.2 m), as this is the required formula to obtain an angle for triangles, this in turn gave me an angle of 56.31 degrees in the bottom left of the triangle. For the inverted triangle I did roughly the same thing, however I had to cut 0.4 m away from roller B so that way it would end up as a right triangle. Know that it was cut properly I took arctan (0.3 m/0.4 m) and obtained 36.86 degrees in the upper left corner of the triangle. Now that I had the angles all I needed was the reactions at B and A so I could begin finding internal loads in all my members. So, to obtain the reaction at A I had to take a moment about roller B; MB=0= (0.04 m)(3)(Ay)+20 kN(0.4 m)-20 kN(0.8 m), this in turn gave me a reaction of roughly 6.67 kN=Ay. Now since all loads were applied in the y-direction I can assume that Ax=0 since nothing pushes or pulls in that direction. Now that I have my first reaction I can easily obtain my second by taking a sum of all forces in the y-direction; Fy=0=By+6.67 kN+20 kN-20 kN, this in turn gave me a reaction of -6.67 kN=By. Now that I had the angles and reactions at both A and B I could finally start solving for my internal loads in all my truss members.

   -_Internal Loads_

<img width="3024" height="3203" alt="IMG_3346" src="https://github.com/user-attachments/assets/495bf4e0-7ddb-47cf-a8e2-01730ec9cdaa" />

To begin calculating my internal loads I had to choose a spot that would statically determinate, so I choose joint B as it had one known and two unknowns which makes it possible to solve for the internal loads as it is statically determinate there. I took a sum of all the forces in the y-direction to start; Fy=0=-By-BC sin(36.86), which rearranged to solve for joint BC becomes; BC=-BY/sin(36.86), I plugged in my numbers and got BC=11.12 kN in compression. So now that joint BC was solved, I could find joint BE by taking a sum of all forces in the x-direction; Fx=0=BE+BC cos(36.86), which rearranged to solve for BE becomes; BE=-BC cos(36.86), putting the numbers in gave BE=8.897 kN in tension.

<img width="2805" height="2908" alt="IMG_3347" src="https://github.com/user-attachments/assets/2e051bca-5542-4ee1-bc88-36ddfe90f090" />

Now that I solved joint B I could move onto joint C to find the final internal loads of the truss due to it being symmetric. So, to start things off I took a sum of all forces in the y-direction again; Fy=0=CE sin(56.31)-BC sin(36.86)+P, when I rearranged this one to solve for CE it came out like this; CE=-(P+BC sin(36.86)/sin(56.31), and after I put the numbers in it gave me CE=16.02 kN in compression. Now that I have joint CE solved, I could now take a sum of the forces in the x-direction to find CD; Fx=0=CD-CE cos(56.31)+BC cos(36.86), which rearranged to solve for joint CD becomes; CD=CE cos(56.31)-BC cos(36.81), after plugging in the numbers I obtained CD=0 kN which means that joint CD is a zero force member. It also means in the design of my truss I technically would not need joint CD for the truss to be structurally sound. So now that I found all the internal loads on the left side the truss I could find them on the right, but as stated before there is no need since the truss is symmetric. Since the loads push in opposite this means each joint on the right has opposite sign internal loads so joint AD=11.12 kN in tension, joint AE=8.897 kN in compression, and joint DE=16.02 kN in tension.

-_Area and Weight of Truss_

<img width="2560" height="3933" alt="IMG_3348" src="https://github.com/user-attachments/assets/6d1abb35-9f52-4b6d-af97-3d77055d11a4" />

Now that I had figured out all the internal loads on my truss, I could calculate the area of the bars to know how thick to make them. The only way to get the area of the bars was to take the largest internal load on my truss, a factor of safety of 3.5, and the material properties for my truss and use them in the FOS/Stress equation to determine the area that each bar needs to be. Since there was no A500 structural steel I had to go with the next best thing which was ASTM A36 steel which was pretty similar to A500 having a density of 7850 kg/m^3 and a yield stress of 250 MPa. So now that I know my material properties, I can find the actual stress that is affecting my truss and use that with the largest internal load to determine a proper area for my bars. So, we will first use the FOS equation to find the actual stress; FOS=yield/actual, and when rearranged to solve for actual gives; actual=yield/FOS, after plugging my numbers in I got 71.43 MPa as the actual stress that affects my truss. Now I could find the proper area and on top of that a proper diameter as well; actual=F/A, of course when rearranged to solve for A turns the equation into; A=F/actual, and after putting my numbers in I arrived at an area of 224.28 mm^2. With that area we can reverse the area equation of a circle; A=pi(r)^2, rearranged to solve for radius; r=sqrt(A/pi), and plugging area into that equation gave me a radius of 8.45 mm. Obviously doubling the radius gave the diameter of the bars which I would have to make 16.9 mm in diameter due to the area I found based on the actual stress.

<img width="2973" height="2322" alt="IMG_3349" src="https://github.com/user-attachments/assets/a0aaebbf-f210-422f-a2d9-40040e58ac0a" />

 The next thing to do was to find the weight of the entire truss without the pins in them
