# A6 – Bracket Drawings

## **Objective**

-Parametrically design both versions of the A5 Bracket based on the equations of stress and deformation

-Put said models into a drawing, with correct diemensions, tolerences, and correct angle projection

-Detail any mistakes through the process

-Create a reflections section

-Time taken on assignment

## **Parametric Designs**

I had previously designed the models with parametrics in mind with the last assignment A5-Bracket Design, so for both models I'll be pulling references from the previous assignment since part of this assignment requires designing the models parametrically. 

_Parametric Based on Stress Analysis_

<img width="355" height="402" alt="image" src="https://github.com/user-attachments/assets/15d872aa-9db0-46af-bc1c-1ccfb92c412f" />

This is the model of the bracket based on stress analysis, where no deformation was previously specified, meaning I had to solely use stress equations when determining the dimensions of features A through E.

<img width="1201" height="341" alt="image" src="https://github.com/user-attachments/assets/1f7bf457-020f-4c57-b861-7b26339bef83" />

This picture here shows each feature parametric equation which was used to help make the model of the bracket. So, starting out with feature A, which was determining the radius/diameter of the cylinder meant to hold up the force of strap, I used the provided equation and assumption from the assignment hints and was able to create a full equation for feature A to define the diameter of the cylinder based on the 600-pound force I had chosen in the previous assignment. The diameter for the cylinder came out to be 20.89 mm which would be more than enough to hold up the distributed force across feature A. With feature A defined allowed me to move onto feature B which was the connection between the fit around the Rigid-T beam and the cylindrical overhang holding up the strap, I yet again used the assumptions from the hints section on the assignment and the diameter of feature A to help me determine the height of feature B, which came out to be 3.72 mm. The reason I used the diameter of feature A here is that it acted as the base for feature B allowing to me to go ahead and pre-define something and make it easier for me to determine the height of the feature. Moving onto feature C the equation for this one took me a second to rearrange for the length since I was trying to combine the bending stress equation with the Factor of Safety equation, which would allow me to just have one parametric equation for feature C instead of two. After I got the equation rearranged, I used the assumptions again from, and with the dimensions from the Rigid-T beam I was able to get the length of feature C to be 17.90 mm which made the feature come out pretty thick. However, this was intentional since we had assumed that feature C was a simply supported beam with a concentrated load in the middle. Now with feature C completed it was time to move onto the second to last feature, feature D. Since there were no predefined assumption hints for feature D in the assignment, I decided to treat feature D the way I treated feature B, which was a purely axial based load. With that assumption and with the dimensions of the Rigid-T beam I was able to obtain the base of feature D by rearranging the stress equation, this in turn gave me a base of 1.02 mm. Last and certainly not least was feature E, and this one was a bit tricky as it also did not have an assumption hint predefined in the assignment, this in turn made it hard to determine its length. I decided to use the same equation we used for C to help determine the length of E, and since some of the dimensions of E were already defined it made it a bit easier to determine the length which came out to be 11.32 mm.

_Parametric Based on Stiffness Analysis_

<img width="387" height="517" alt="image" src="https://github.com/user-attachments/assets/cbf232ce-6344-4e93-81de-7c50a15bae5f" />

This is the model of the bracket based on stiffness analysis, where deformation was specified to be about 0.005 in, meaning I had to solely use deformation equations when determining the dimensions of features A through E.

<img width="1365" height="339" alt="image" src="https://github.com/user-attachments/assets/decac0e3-2e80-4b54-a7fc-2be8059771c0" />

This picture here represents the same geometric features I was trying to find, but now it's using the deformation equations for axial loads and beams. All of these dimensions came out smaller than their stress analysis counterparts especially feature D and B which came out too 0.18 mm and 0.46 mm respectively. I still used the same assumptions for features A-E and based some of the features around the dimensions of the Rigid-T beam and the strap. This model would break/fracture/crack under the applied 600-pound load due to the fact that all the equations used here were based using a deformation of 0.005 in. With this in mind it would definitely be better to use the bracket that was designed with stress analysis in mind as it contains dimensions with much greater values than the ones based on stiffness analysis.

## **Drawings**

_Stress Analysis Drawing_

<img width="1119" height="865" alt="image" src="https://github.com/user-attachments/assets/b3974650-2d6d-40aa-906f-f29df20402fc" />

This is the drawing of the Bracket with stress analysis in mind, I made sure to add the center mark and center lines in the appropriate views and set the multiview to have hidden lines present, I also made sure to add appropriate dimensions to each view accordingly. On top of this I added the Third Angle Projection Symbol since this drawing will be based with AMSE in mind, gave the drawing a title and number, added what material was used, added an isometric in the top right of the multiview, added tolerances for one, two, and three decimal places, added a date and name of who it was drawn by, and lastly changed the dimension format to inches to match up with the Third Angle Projection Symbol.

_Stiffness Analysis Drawing_

<img width="1141" height="880" alt="image" src="https://github.com/user-attachments/assets/5a86d259-e02a-4b93-96a3-45872c28c3dc" />

This is the drawing of the Bracket with stiffness analysis in mind, I made sure to add everything previously added in the stress analysis-based drawing such as the center mark, center lines, hidden lines, Third Angle Projection Symbol and etc. Obviously, some of the dimensions are smaller here due to using deflection-based equations instead of stress-based equations.

## **Reflections**

One parametric equation I used was for feature B on the stress analysis side, the equation used for feature B was used to determine the height of B, using a combination of the normal stress equation with the Factor of Safety equation and the diameter of feature A. The way I was able to do this was by setting the Factor of Safety equation equal to the normal stress equation, then by breaking the area in base and height, I could isolate the height portion to solve for it. As stated earlier the base was already predetermined as feature B's base needed to cover over feature A, so the best way to do that was to take the diameter of A and use that as the base for feature B. Well, if the calculation changed, say like if the Factor of Safety changed or I chose a different force, then I would get an entirely different value for the height of B, changing the height of B would not have any affect on any other feature within the model as no other feature has the height of B in their parametric equation.

A couple places that I had to apply tighter tolerances was around the main cavity area of the bracket where it fits onto the Rigid-T beam, I needed the tolerances to be tight there to prevent the bracket from being too loose of a fit onto the beam and also preventing it from being not big enough to fit onto the beam. So, by applying a tighter tolerance to those regions in particular it makes sure that the bracket will fit well onto the Rigid-T beam. As for some of my other dimensions say the height or width of the bracket those would not matter as much as they are not making contact onto anything or trying to fit onto to something so they have looser tolerances compared to some of my other dimensions like the part that has to fit around the Rigid-T beam.

## **Lessons Learned**

A good lesson I learned in this assignment is knowing which dimensions in the drawings need looser or tighter tolerances. As just stated in the reflection, something like the height of the bracket can be given a loose tolerance as it does not make contact with anything or fit around something allowing for the tolerance to be loose. On the other hand, the internal cavity where the bracket fits around the Rigid-T beam need to have tighter tolerances so it can fit properly around the beam otherwise if the part is manufactured with a loose tolerance it most likely will not fit properly onto the Rigid-T beam.

## **Time Taken on Assignment**

The overall time it took me to complete this assigmnent was around three hours.

## **Model/Drawing Links**

I am deciding to provide the model links again from A5

https://drive.google.com/drive/folders/1h2l4XzkjOTJ58OEj_yXmsrLULNwk89K0?dmr=1&ec=wgc-drive-%5Bmodule%5D-goto
