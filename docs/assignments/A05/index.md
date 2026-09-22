# A5 – Bracket Design

## **Objective**

-Conduct stress analysis to determine appropriate dimensions for structural features.

-Generate free body diagrams (FBDs) to visualize forces and constraints for each feature.

-Identify and document known and unknown variables, assumptions, and algebraic models for stress calculations.

-Perform stiffness analysis to establish minimum required dimensions based on deflection constraints.

-Compare stress and stiffness analyses to ensure structural integrity and compliance with given constraints.

-Create detailed multiview sketches illustrating dimensions derived from both stress and stiffness analyses.

-Reflect on and document key engineering lessons learned throughout the process.


## **Diemensions Based on Stress Analysis**

_Feature A_

<img width="2674" height="3324" alt="IMG_3432" src="https://github.com/user-attachments/assets/615b3cf4-faca-4e57-b408-449870b8aa6c" />

So, for feature A I had to assume that it was a cantilever beam experncing no shear with a distributed load of F2 applied across it based on the dimensions of the strap, force, Factor of Safety, material, and its properties. The material I choose was 6061-T6 Aluminum which has a Young's Modulus of 69000 N/mm^2 and a Yield Strength of 275 N/mm^2, I also decided to use a 600-pound force applied to the feature which converted to SI gives 2668.93 N. That force of 2668.93 N times two gave me 5337.87 N of force being applied to feature A. What I had to find was the area of feature A and the radius of feature A, on top of that I also went ahead and predetermined the length of feature A, to be 23.05 mm, based on the dimensions of the strap which were given in the assignment. The reason I made feature A longer than the width of the strap was to give a little bit of extra clearance on both sides so that way the strap was not rubbing up against feature B, but to also prevent it from slipping off the edge of feature A.

<img width="2777" height="1466" alt="IMG_3433" src="https://github.com/user-attachments/assets/8dfcf3a5-8f2a-4347-9c5f-a4eb226cc02e" />

Based on the equation given to us to determine the radius of feature A, and with everything else that was predetermined or chosen, I arrived at a radius of 10.44 mm which multiplied by two gave me a diameter of 20.88 mm. I was able to obtain this diameter by first determining what Z was which was 894.82 mm^3, then by using that Z I plugged it into the equation for the radius of the feature which landed me at the 10.44 mm.

_Feature B_

<img width="2634" height="2276" alt="IMG_3433 (1)" src="https://github.com/user-attachments/assets/6c83b917-0bc3-4f4b-9bb1-ba39e3120815" />

Moving to feature B, for this scenario I had to assume that it was purely axially loaded and that there was no shear. I decided to make the base of feature B the same as the diameter of feature A, 20.88 mm, this way feature B would fit perfectly flush into feature A and allow for a smooth transition for the force F to move through. This time however instead of determining the radius of a feature I had to instead determine the length, height, area, and actual stress of the feature and all this would depend upon the stress/FOS equation, and the dimensions of the strap.

<img width="2446" height="3042" alt="IMG_3434" src="https://github.com/user-attachments/assets/d6fb23d8-8383-4da8-9c72-a2fadaf55516" />

To determine the actual stress affecting feature B I used the FOS equation and rearranged to solve for the actual stress, stress actual=yield strength/FOS, plugging in the numbers for both variables gave me an actual stress of 68.75 N/mm^2. Then with the actual stress acquired I could rearrange the stress equation for area, A=F/actual stress, which after putting the numbers in yielded an area of 77.64 mm^2. Then with area I could break it down into base time height which rearranged to solve for height gave me this equation, h=A/b, then after putting in the numbers for the area and the base gave me a height of 3.72 mm. For the length of feature B I decided to use the dimensions of the strap again on top of the radius of feature A, and also adding in a bit of extra clearance. This gave me an equation as such, strap thickness+radius of feature A+1.75 mm extra clearance, once I put the numbers into the equation, I had a total length of 13.384 mm. The reason I used this equation as to determine the length of feature B was so that way the strap would not rub against the underside of feature C. 

_Feature C_

<img width="2379" height="3272" alt="IMG_3435" src="https://github.com/user-attachments/assets/10a43cb7-df7d-40ec-9575-b6831b511d1d" />

<img width="2357" height="2864" alt="IMG_3437" src="https://github.com/user-attachments/assets/9c58b0aa-d723-499a-a4e0-7b1891f607bb" />

Moving on to feature C, I assumed this feature as a simply supported beam experiencing no shear subjected to a central point load of 5,337.87 N applied through feature B. The total span width between the inner walls was determined to be 63.41 mm, and the length was kept constant at 23.05 mm to match the overall length of the bracket. To obtain the height of feature C, I used the maximum bending moment equation for a simply supported beam with a center load, M=Fl/4. Then with the moment portion defined I could use the bending stress equation to determine the height of feature C, the equation is as follows, stress=(M* h/2)/(bh^3/12). After simplifying the equation and rearranging for height I got this equation, sqrt((6*M/stress)/b), then once I put the numbers in, I arrived at a height of 17.90 mm.

_Feature D_

<img width="2569" height="3370" alt="IMG_3436" src="https://github.com/user-attachments/assets/d21344ef-7a9e-4f0c-afdb-049522db6249" />

For feature D, this corresponds to the vertical side walls connecting Feature C to Feature E. Looking at the bracket geometry, the part is symmetric with two identical side walls carrying the load together in parallel. Because the total force of 5,337.87 N is shared equally between both walls, the force acting on one wall is, F=P/2= 2,668.93 N. Assuming pure axial loading again with no shear, I determined the base of feature D using the stress equation, stress=F/A. Rearranging to solve for the Area gave me this equation, A=F/stress, which after plugging in the numbers gave me an area of 38.83 mm^2. Then rearranging the area equation for base and plugging in the numbers yielded a base of 1.02 mm. 

_Feature E_

<img width="2482" height="3198" alt="IMG_3438" src="https://github.com/user-attachments/assets/e2e7d09f-c54b-4d20-b422-bdfeb8e7667b" />

<img width="2287" height="2385" alt="IMG_3439" src="https://github.com/user-attachments/assets/ed0a8b11-3b1b-40b3-a21e-3e6e114ffb14" />

_Multiview Sketch_

<img width="2793" height="3525" alt="IMG_3448" src="https://github.com/user-attachments/assets/2208d31d-b1f2-405f-81b1-826d31ff80cd" />

Here is the Multiview sketch with three views, front/right/top, and fully dimensioned with hidden lines and center lines.

_CAD Model_

<img width="689" height="656" alt="Screenshot 2026-09-22 060845" src="https://github.com/user-attachments/assets/2df1b980-fd3a-4322-8fa2-c75bf77bf93c" />

Here is the full 3-D CAD model made in SolidWorks with correct material properties and designed using some parametric equations.

## **Diemensions Based on Stiffness Analysis**

_Feature A_

<img width="2304" height="2923" alt="IMG_3440" src="https://github.com/user-attachments/assets/46f6d46f-3679-43bc-9035-66c98bc1cf7c" />

<img width="2435" height="2611" alt="IMG_3441" src="https://github.com/user-attachments/assets/3604c56a-9fb2-4856-bc04-712a6857ce39" />



_Feature B_

<img width="2508" height="3058" alt="IMG_3442" src="https://github.com/user-attachments/assets/2fca1199-46d9-4777-8aea-8fd12f38b08a" />

<img width="2265" height="1390" alt="IMG_3443" src="https://github.com/user-attachments/assets/9a2d6781-9ca2-4f92-be15-82c7f1be4ed9" />



_Feature C_

<img width="2326" height="3104" alt="IMG_3444" src="https://github.com/user-attachments/assets/998936ac-b7a3-491c-8e7b-d35ad237a411" />

<img width="2398" height="1133" alt="IMG_3445" src="https://github.com/user-attachments/assets/376a6847-5559-4a19-bf1e-5606b2c7b64b" />



_Feature D_

<img width="2414" height="3316" alt="IMG_3446" src="https://github.com/user-attachments/assets/58195141-e706-4d84-b7ee-6b5b51e7928b" />



_Feature E_

<img width="2637" height="3561" alt="IMG_3447" src="https://github.com/user-attachments/assets/44f07f71-b55c-449c-87d2-0f79e2963306" />

_Multiview Sketch_

<img width="2646" height="3331" alt="IMG_3449" src="https://github.com/user-attachments/assets/d08d90dd-b56a-43b7-951a-00ea1501dd79" />

Here is the Multiview sketch with three views, front/right/top, and fully dimensioned with hidden lines and center lines. Due note since feature D was so thin I drew it as a single line, but I still applied its base dimensions.

_CAD Model_

<img width="638" height="637" alt="Screenshot 2026-09-22 060824" src="https://github.com/user-attachments/assets/cb15fd9c-14e5-40c0-ab0e-740915af6abf" />

Here is the full 3-D CAD model made in SolidWorks with correct material properties and designed using some parametric equations.

## **Lessons Learned**

## **Time Spent on A5**

## **Link to CAD Model**
