# A4 – Motor Mount

## Objective

Design a motor mount using the (Brushed 24V DC Gear Motor 3.6Kg.cm/46RPM w/ 99.5:1 Planetary Gearbox) HERE which attaches to the rigid wall A. For both features, first design for yield strength and then design for a maximum deflection of .30 mm at the free end. You may select ABS, PETG,  or PLA as a motor mount material.  When designing the motor mount take into account a safety factor of 3 and neglect the weight of the motor. For steps 1 and 2 draw a FBD of the forces and a concept of your design. Research the design of different motor mounts and place the links in an appendix on your page. Make justifiable approximations in your design to simplify your analysis. (ie. use the beam calculations) Follow Appendix B for the initial approach to set up the design analysis.

## **Feature 1**

_Knowns and Unknowns_

<img width="2609" height="2417" alt="IMG_3424" src="https://github.com/user-attachments/assets/bf675c89-b9bf-4397-9e27-ede7bf946009" />

So, some of the knowns and decisions for feature one that I had made includes the following: E=2.0 GPa, P=300 N, Material of Choice-ABS, Max Deflection=0.3 mm, Yield Stress=30 MPa, Factor of Safety=3.0, Weight of the motor is negligible, making the length of feature one 48 mm, and the height 10 mm respectively. There were not a lot of unknowns as I really only had to determine the area and base of feature from both the beam bending equation and the bending stress equation. I also decided to split up the mount in the same way it appears in appendix B to help me get a start in the design process of the mount.

_Free Body Diagram_

<img width="2589" height="1245" alt="IMG_3424 (1)" src="https://github.com/user-attachments/assets/7ca7c76a-df54-40a0-96b5-1522a30061b3" />

Here is the FBD of feature one with the applied height, length, and force. Since I had already determined the height of feature one it allowed me to determine how much of the shaft stuck out of feature one allowing me to calculate a moment being applied onto feature one. I was able to determine how much shaft stuck out by taking the shafts length of 16 mm and subtracting it from the height of feature one which was 10 mm, 16 mm-10 mm = 6mm, this in turn left me with 6 mm of shaft sticking out of feature one and this in turn allowed me to calculate a moment acting on feature one, M = 6 mm * 300 N = 1800 N*mm. I also went ahead and put the reaction force (Ry) and reaction moment (MR) to complete my entire FBD of feature one.

_Equations_

<img width="2758" height="2869" alt="IMG_3425" src="https://github.com/user-attachments/assets/4efe0e2e-8c45-4cec-a614-b2be38507446" />

I only had to use three equations here the Factor of Safety equation (FOS= stress yield/stress actual), bending stress equation (stress actual=(M(h/2))/I total), and the beam bending equation (deformation=(M*L^2)/2(E)(I total)). I decided to start off with the bending stress equation and try to incorporate the FOS equation into it to make a more simplified equation that would give me a value for the base (b). So, I rearranged the whole equation while also incorporating the hole the shaft made to make the base a little more accurate and I ended up with, b=(12/h^3)((M(h)(FOS)/2(yield stress))+(pi(d)^4)/64), then after plugging in my previously known values I ended up with a b=11.56 mm. 

<img width="2688" height="2227" alt="IMG_3426" src="https://github.com/user-attachments/assets/e46ca15b-b54b-4b68-a501-4e5a019a0529" />

Now it was time to do the same for the beam bending equation and obtain a value for the base of feature one. So, I rearranged the beam bending equation to solve for b and ended up with, (12/h^3)((M*L^2)/2(E * deformation) + ((pi)(d^4)/64))), then after putting my numbers into the equation I ended up with a much larger base compared to the one I obtained in the beam bending equation b=42.24 mm. This is where the choice happens, do I take the smaller area from the bending stress equation or do I take the larger area from the beam bending equation. I obviously took the larger area as the smaller area is just the bare minimum while the larger area gives my motor mount a lot more room to breathe, stress/force wise that is since there is more area for the force to cover.

## **Feature 2**

_Knowns and Unknowns_



## **Sketch**


## **Cad Model**


## **Time Spent**

