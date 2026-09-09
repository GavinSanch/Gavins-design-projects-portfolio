# A3 – Parametric and FEA

## **Objective**

-Use axial deflection modeling to design its dimensions

-Use parametric design to determine a bars length

-Introduce you to FEA (Finite Element Analysis)

-Introduce you to linking dimensions to appropriate parameters in CAD.

-Compare and contrast the different analysis

## **Deciding**

<img width="2463" height="2844" alt="IMG_3411" src="https://github.com/user-attachments/assets/b575146b-7e1a-4f77-ba23-82da52d4fe3c" />

So, for my beam I decided to go with a circular cross-sectional area of 36mm^2 (diameter of 6.77mm). I also decided to go with the strongest load this time of 500 lb., which is roughly 2224.11 N, instead of going with the smallest like I did in A2. I decided to go with 6061-T6 Aluminum as it has a decent yield strength, (275 MPa), and Young's Modulus, (69000 MPa), compared to the other materials within in SolidWorks.

## **Calculating**

_Stress on the Beam_

<img width="3024" height="1173" alt="IMG_3404 (1)" src="https://github.com/user-attachments/assets/5a1ed0df-1bc5-4c5c-98c4-9ddcea454e0a" />

I used the stress formula to get a calculation of how much stress that would be affecting my circular beam, stress=F/A, and after plugging in the numbers I obtained 61.781 MPa of stress acting upon my circular beam with my chosen force and area. I will use this calculated stress and compare to the FEA that I will run later in SolidWorks.

_FOS of the Beam_

<img width="2766" height="827" alt="IMG_3408" src="https://github.com/user-attachments/assets/660dc78a-8e6c-4c78-9380-ed3f500a156f" />

After obtaining the stress acting upon my beam, I could calculate the Factor of Safety on my beam by using, FOS=yield stress/actual stress, then I put in the numbers and got a FOS of 4.45 which is pretty good and means that my beam could withstand a lot more force before yielding and then fracturing.

_Parametric Equation for the length of the Beam_

<img width="2666" height="1475" alt="IMG_3407 (1)" src="https://github.com/user-attachments/assets/95c43a12-8f3e-46b6-b0c6-1c0625a2cf6f" />

By using the deflection equation, I could determine the length of the bar then use that same equation as a parametric equation to put into SolidWorks to tell it how long to extrude the beam. The formula, deflection=FL/EA, and after plugging my numbers in I obtained a length of 255.31 mm.

## **CAD**

_Model of Beam_

<img width="1919" height="1031" alt="Screenshot 2026-09-08 213919" src="https://github.com/user-attachments/assets/be40aa31-f6bc-4463-9e0c-5ff3a53d0f89" />

This is the CAD model of the circular beam I created from the cross-sectional area of 36mm^2 and with the parametrized equation that I made from the deflection equation.

_Deflection Map of Beam_

<img width="1919" height="1031" alt="Screenshot 2026-09-08 214021" src="https://github.com/user-attachments/assets/cf15b218-6e0a-40c8-8327-c26186bde337" />

This is the deflection map of my circular beam, as you can see from the image red is the place where there is the most deflection on my beam and blue is where there is the least amount of deflection on my beam. The way I set this up was applying a fixture at one end of the beam, placing in the 2224.11 N force at the other end of the beam, applying the 6061-T6 material properties to the beam, then running the simulation to obtain the results. Now something I did notice was that the max was off by 0.0002 mm which is a pretty small difference between what the simulation calculated and what I calculated. 

_Von Mises Stress Map of Beam_

<img width="1919" height="1032" alt="Screenshot 2026-09-08 214029" src="https://github.com/user-attachments/assets/03793bf8-fb9c-4f83-8944-46392ad4f7aa" />

This is the Von Mises map on my beam, and as you can see from the image the entirety of the beam sits in the yellow region between 58.08 MPa and 62.51 MPa which is pretty accurate for my calculated stress of 61.781 MPa. Sadly, I cannot determine the actual stress in the simulation as SolidWorks lacks any sort of "probe" feature to allow me to see the stress acting at any point along the bar. The best part is that my circular bar sits well below the yield strength of the material further proving my calculation was correct.

_Factor of Safety Map of Beam_

****<img width="1919" height="1032" alt="Screenshot 2026-09-08 214013" src="https://github.com/user-attachments/assets/2ec1e9c6-9506-4e86-abee-4e7fc92589cf" />

This is the Factor of Safety map on my beam; I decided to set the FOS higher than its standard of 1 to show how my beam's calculated FOS was up to at least 4 since I calculated it had an FOS of 4.45.

## **Design Reflection**
a.)
So the axial deflection from my calculations was 0.2286mm while the one in the FEA was 0.2284mm, these two values are practically similar, and it comes down to the parametric length equation I used to determine the correct length of my circular bar, the chosen cross-sectional area, and the applied force of 2224.11 N. These three things allowed for my deflection in both calculation and in the FEA to be almost identical to each other due to these determined and predetermined factors. Now as for the percent difference between the two, |calculated-FEA/calculated| X 100%, and after plugging in the numbers I ended up with a 0.0874% difference.

<img width="2792" height="1393" alt="IMG_3408" src="https://github.com/user-attachments/assets/59a37d17-ef42-4a24-b9c5-68142c8b8236" />

b.)
If there were a substantial pin hole placed on my bar the stress concentration factor (Kt) would be 2.5 based on the charts in the Machineries Handbook. The equation for max stress goes as follows, max stress=Kt X nominal stress, so putting the numbers in gave me a max stress 154.4525 MPa directly at the pin hole. This would for sure pass my safety factor as this peak stress still sits about halfway under my materials yield strength, as the new FOS would be 1.78 which sits a bit lower than my originally calculated FOS of 4.45, however it still sits above one which is a design standard for all parts.

## **Engineering Lesson Learned**

I feel like an engineering lesson I learned was how to parametrize a part based on an equation, as parametrization allows us engineers to change the length, area, diameter, radius, etc. through just a couple of numbers instead of having to always edit a sketch or feature on the part. Using an equation allows one to easily change the numbers in it to change how the part will look and it takes no time what so ever, which helps the design process smooth and streamlined.

## **Time Spent on A3**

I believe the total time that I spent working on A3 was about 4 to 5 hours total.
