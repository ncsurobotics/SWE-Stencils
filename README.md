# SWE-Stencils

## In order to make a stencil:
 1. Create a new PCB project with the year and month of the stencil order
 2. Create a readme.md with the PCBs you plan to have on the stencil listed inside the project folder
 3. Make sure the SW-Altium-Libraries is up to date on your local computer
 4. Pull all of the PCB repos you plan to use for this stencil
 5. Create a new .PCBDOC with the project name inside the new project folder
 6. Make the board size about 100mm by 90mm max
    * Board can be larger but will result in higher stencil cost/shipping
 7. Copy and paste PCBs that you want to be on the stencil into the new .PCBDOC
    * Don't worry about through hole components as they aren't needed for the stencil
    * Don't feel required to have all of the components on the stencil. Focus on complicated/difficult to solder areas
    *If you want pads that are on the back of the PCB: 
      * Make a copy of the needed components
      * Paste the components far off the board so you can easily reselect them
      * Highlight the components and start dragging them as if you're trying the move them
      * Press L on your key board to flip/mirror the components onto the top layer
      * Move the components where you want them to be laid out
 8. Arrange PCBs in ways that make sense and don't overlap
 9. Once done save and commit all of your new changes
10. Click on File > Fabrication Outputs > Gerber Files
    * May have to click generate Output
11. Go to the Layers tab in the dialog box that appears
12. Make sure that only the "Top Paste" layer is checked to plot
13. Press Ok 
    * A .Cam file should appear with all of the places that you want solder paste to be
14. Check the .Cam file to make sure all of the important components generated properly
15. Zip the .GTP file (Found in the "Project Outputs for <Project Name>" folder) into its own .zip folder 

## Ordering a Stencil
1. Go to <a href="https://www.jlcpcb.com">jlcpcb.com</a>
2. Click on SMT Stencil Quote Now
3. Add the .zip file where it says to Add gerber file
4. Check that the preview looks right
5. Fill out options (Feel free to edit but this generates minimal cost)
  * Framework: No
  * Step Stencil: No
  * Dimensions: Smallest size (380mmx280mm)
  * Customized size: Yes
    * x: 100mm
    * y: 90mm
  * Stencil Side: Top
  * Stencil Qty: 1
  * Polishing Process: Depends on use case
  * Fiducials: No Fiducial
  * Confirm Production File: Your Choice
  * Engrave Text: Yes
    * Stencil Remark: 
      <p> NCSU URC SW8 - Month Year<br>
      "Repo Used" Rev \#.\#<br>
      "Repo Used" Rev \#.\#<br>
      ...</p>
6. Check the preview again
7. Save to Cart

