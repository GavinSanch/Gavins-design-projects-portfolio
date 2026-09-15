# A4 – Motor Mount

## Objective

Design a motor mount using the (Brushed 24V DC Gear Motor 3.6Kg.cm/46RPM w/ 99.5:1 Planetary Gearbox) HERE which attaches to the rigid wall A. For both features, first design for yield strength and then design for a maximum deflection of .30 mm at the free end. You may select ABS, PETG,  or PLA as a motor mount material.  When designing the motor mount take into account a safety factor of 3 and neglect the weight of the motor. For steps 1 and 2 draw a FBD of the forces and a concept of your design. Research the design of different motor mounts and place the links in an appendix on your page. Make justifiable approximations in your design to simplify your analysis. (ie. use the beam calculations) Follow Appendix B for the initial approach to set up the design analysis.

## **Feature 1**

_Knowns and Unknowns_

<img width="2609" height="2417" alt="IMG_3424" src="https://github.com/user-attachments/assets/bf675c89-b9bf-4397-9e27-ede7bf946009" />

So, some of the knowns and decisions for feature one that I had made includes the following: E=2.0 GPa, P=300 N, Material of Choice-ABS, Max Deflection=0.3 mm, Yield Stress=30 MPa, Factor of Safety=3.0, Weight of the motor is negligible, making the length of feature one 48 mm, and the height 10 mm respectively. There were not a lot of unknowns as I really only had to determine the area, base, and actual stress of feature one from both the beam bending equation and the bending stress equation. I also decided to split up the mount in the same way it appears in appendix B to help me get a start in the design process of the mount.

_Free Body Diagram_

<img width="2589" height="1245" alt="IMG_3424 (1)" src="https://github.com/user-attachments/assets/7ca7c76a-df54-40a0-96b5-1522a30061b3" />

Here is the FBD of feature one with the applied height, length, and force. Since I had already determined the height of feature one it allowed me to determine how much of the shaft stuck out of feature one allowing me to calculate a moment being applied onto feature one. I was able to determine how much shaft stuck out by taking the shafts length of 16 mm and subtracting it from the height of feature one which was 10 mm, 16 mm-10 mm = 6mm, this in turn left me with 6 mm of shaft sticking out of feature one and this in turn allowed me to calculate a moment acting on feature one, M = 6 mm * 300 N = 1800 N*mm. I also went ahead and put the reaction force (Ry) and reaction moment (MR) to complete my entire FBD of feature one.

_Equations_

<img width="2758" height="2869" alt="IMG_3425" src="https://github.com/user-attachments/assets/4efe0e2e-8c45-4cec-a614-b2be38507446" />

I only had to use three equations here the Factor of Safety equation (FOS= stress yield/stress actual), bending stress equation (stress actual=(M(h/2))/I total), and the beam bending equation (deformation=(M*L^2)/2(E)(I total)). I decided to start off with the bending stress equation and try to incorporate the FOS equation into it to make a more simplified equation that would give me a value for the base (b). So, I rearranged the whole equation while also incorporating the hole the shaft made to make the base a little more accurate and I ended up with, b=(12/h^3)((M(h)(FOS)/2(yield stress))+(pi(d)^4)/64), then after plugging in my previously known values I ended up with a b=11.56 mm. 

<img width="2688" height="2227" alt="IMG_3426" src="https://github.com/user-attachments/assets/e46ca15b-b54b-4b68-a501-4e5a019a0529" />

Now it was time to do the same for the beam bending equation and obtain a value for the base of feature one. So, I rearranged the beam bending equation to solve for b and ended up with, (12/h^3)((M*L^2)/2(E * deformation) + ((pi)(d^4)/64))), then after putting my numbers into the equation I ended up with a much larger base compared to the one I obtained in the beam bending equation b=42.24 mm. This is where the choice happens, do I take the smaller area from the bending stress equation or do I take the larger area from the beam bending equation. I obviously took the larger area as the smaller area is just the bare minimum while the larger area gives my motor mount a lot more room to breathe, stress/force wise that is since there is more area for the force to cover. This equation will be used as a parametric equation later for my CAD model.

## **Feature 2**

_Knowns and Unknowns_

<img width="2280" height="1413" alt="IMG_3427" src="https://github.com/user-attachments/assets/bf1cc5c5-9f37-4f5d-87fe-c13c7e72fd5b" />

For feature two, which is the part of the mount that is partially fixed and partially free, had a decent number of knowns and decisions: b=42.24 mm, E=2.0 GPa, h=7 mm, Max Deflection=0.3 mm, FOS=3, Yield Stress=30 MPa, P=300 N, Bolt Holes=3.4mm.
There were only three unknowns again just like for feature one: Free Length, Fixed Length, and actual stress.

_Free Body Diagram_

<img width="2598" height="450" alt="IMG_3427 (1)" src="https://github.com/user-attachments/assets/a0ecd1e1-7a4e-453b-93f9-7f550c64d7bf" />

The FBD of feature two was nothing special as I assumed yet again that it acted as a cantilever beam just how I assumed in feature one that it was a cantilever beam. I included the moment that was calculated originally from feature one and applied it to feature two to help me determine the lengths of the fixed and freed portions of feature two.

_Equations_

<img width="2664" height="1666" alt="IMG_3427" src="https://github.com/user-attachments/assets/8510e00a-0105-4ac1-ad32-35a83d170fe3" />

My equations were relatively the same the only difference was one extra addition for fixed length (L-Fixed=C*d) and the fact that instead of solving for the base in both equations I would be solving for the free length in each. So, for the fixed portion of the length it was an easy and simple equation just using C=7 and d=3.4 mm which multiplied together gave me a fixed length of 23.80 mm.

<img width="2939" height="3561" alt="IMG_3428" src="https://github.com/user-attachments/assets/08ceae00-1a73-4d5b-aa6c-3c583c2a8568" />

As for the rest equations I just had to rearrange both to solve for L-Free, plug in the numbers and see which one is larger. I yet again started with the bending stress equation and combined it with the FOS equation to help make the equation simplified and help me obtain L-Free with ease. So, after rearranging the bending stress equation to solve for L-Free I ended up with, L-Free=(1/P)((b)(h)^2(yield stress)/6(FOS) - M), after running my known values through the equation I ended up with L-Free=3.65 mm. Now that I had bending stress I could move onto the beam bending equation again which rearranged to solve for L-Free gives, L-Free=sqrt((2E(((b-2(d))h^3)/12)(deformation))/M), and after plugging my numbers in I arrived at L-Free=25.99 mm. So, know that I had both L-Free and L-Fixed I could add them up together to obtain the total length of feature two, total length=25.99 mm+23.80 mm=49.79 mm, I will also use this as another parametric equation for my CAD model.

## **Sketch**



## **Cad Model**


## **Time Spent**

