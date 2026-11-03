# A8 – Gearbox Design

## **Objective**

-Design a gearbox that can be assembled and disassembled.

-Analyze and size input and output shafts for strength.

-Design journal bearings to support shafts.

-Create a gearbox housing with proper clearance and fastening.

-Use parametric CAD modeling to generate a final design.

-Document calculations, sketches, and lessons learned.

## **Assumptions/Notes**

Some of the assumptions/notes we were allowed to assume or take note of while doing this assignment are as follows;

-Assuming the appropriate strength of shafts using machineries handbook.

-That shafts are to be press fitted through the hubs of the gears used in the assignment.

-That the gear train used here in the assignment is ideal meaning there is no losses due to friction or heat.

-That both the pinion and gear have adequate space while in the gearbox housing.

-The moment of radial force generated from the gear train is so small that it can be ignored.

-To use a running sliding fit for the size of the hole for the shafts.

## **Shafts**

These four images lay out FBD's, Calculations, Knowns/Unknowns, and Equations used for determining if both the input and output shaft diameter were adequate enough based on the calculated torsional shear stress. Both shafts had more than efficient diameters based on torsional shear and the factor of safety I calculated, using 1045 steel. I did not however assume the weight of the gear and pinion being applied to the shaft to help not only help keep the calculations simple but to also prevent me calculating the bending stress effecting the shaft due to the weight of the pinion and gear. I also calculated the input torque and input speed, since they will both be necessary for not just these first couple of calculations but also for later calculations.

-_Input Shaft_

<img width="3024" height="4032" alt="IMG_3515" src="https://github.com/user-attachments/assets/2336e137-546e-49df-8c09-d64f7ea5744c" />

<img width="3024" height="4032" alt="IMG_3516" src="https://github.com/user-attachments/assets/826d4895-ada9-441d-b9a2-edb00d148829" />

-_Output Shaft_

<img width="3024" height="4032" alt="IMG_3517" src="https://github.com/user-attachments/assets/1f1e0be4-3067-4f55-bec6-c635017b4f99" />

<img width="3024" height="4032" alt="IMG_3518" src="https://github.com/user-attachments/assets/74db8741-49ad-4bf9-9e27-b9620ca19b33" />

## **Journal Bearings**

These four images show my Calculations, FBD's, Knowns/Unknowns, and Equations used for determining the size, length, and thickness for both my input and output journal bearings. The journal bearings required a little bit more calculating since I needed the tangential force, area, pressure, velocity, and radial force so I could obtain the PV factor for both input and output to help me determine the appropriate material for the bearings which came out to be poupous bronze based on the Machineries Handbook. Thankfully though getting the thickness of both bearings was not as difficult since all it required was assuming the OD of both, and on top of this I decided to include and calculate hoop and radial stress in my calculations. The thickness for both journals came out to be 0.0625 in which is very adequate, this in turn would make the OD-in=0.250 in and the OD-out=0.375 in. The two journal bearings I pulled from McMaster are as follows 6391K111_Oil-Embedded 841 Bronze Sleeve Bearing, for the input bearing, and 6391K131_Oil-Embedded 841 Bronze Sleeve Bearing, for the output bearing, both of which will be used in my CAD Assembly.

-_Sizing and Length of Journals_

<img width="3024" height="4032" alt="IMG_3519" src="https://github.com/user-attachments/assets/5d51c775-6341-4941-ac19-4f4efb5f2253" />

<img width="3024" height="4032" alt="IMG_3520" src="https://github.com/user-attachments/assets/77decc54-118d-47aa-99b0-d08cb12dbd8b" />

-_Thickness of Jounrals_

<img width="3024" height="4032" alt="IMG_3521" src="https://github.com/user-attachments/assets/88919fc8-64f7-4158-a116-d9bd7a8194a5" />

<img width="3024" height="4032" alt="IMG_3522" src="https://github.com/user-attachments/assets/b6df53eb-234a-447e-9662-353abe1cbfaf" />

-_McMaster Journals based on Calculations_

<img width="499" height="713" alt="Screenshot 2026-11-03 072051" src="https://github.com/user-attachments/assets/d5cf765c-4ca3-48e8-b333-194ff6b7c440" />

<img width="500" height="729" alt="Screenshot 2026-11-03 072117" src="https://github.com/user-attachments/assets/9c7a6b23-b48d-4628-8af8-cd586401e62c" />

## **Gearbox Housing Sketch**

This here is just a rough sketch of my Gearbox Housing that I constructed really quickly, I decided to make the housing circular to better fit around the gears and help distribute forces easier compared to a rectangular box. However, as I said this is just a rough sketch and I decided to add extra features in my CAD models. Also, the way I decided to fixate both parts of the housing was with a webbed feature on both ends with six holes to accommodate for six bolts.

<img width="3024" height="4032" alt="IMG_3523" src="https://github.com/user-attachments/assets/be0d31bd-9818-4c32-a456-4e51c86bdbfe" />

## **CAD**

Both of these images here are the outside and inside of the gearbox housing, I decided to apply a couple of material properties to some of the models such as; making both pinion and gear out of brass as stated in their McMaster description, both shafts being made from 1045 steel cold drawn, both McMaster bearing made of 841 Bronze, the gearbox housing made out of ABS. I also added the six bolts, with nuts and washers on both sides of the webbed flange. There was a slight issue that I realized while making the gearbox housing model, since I had placed both pinion and gear in the middle of their shafts, there was a slight 0.03 in offset on either side just to have them properly mesh with each other. This in turn is why my housing sticks out a bit on the gear side. I also decided not to use parametric equations since there was no reason to, the shafts had no defining equations since they were already pre-defined, same goes for the gears, the bearings I decided to download off of McMaster and use them in my assembly directly.

-_Outside of Gearbox Housing_

<img width="958" height="649" alt="Screenshot 2026-11-03 052155" src="https://github.com/user-attachments/assets/67519da8-35d0-467e-9683-2eaa9d15498d" />

-_Inside of Gearbox Housing_

<img width="889" height="591" alt="Screenshot 2026-11-03 052220" src="https://github.com/user-attachments/assets/8e7c7277-f236-4e6c-be2b-9199a1ef241c" />

## **Lessons Learned**



## **Time Taken for Completion**



## **Link to CAD Models**

