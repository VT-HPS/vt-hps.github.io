
# Operating the Waterjet at AEDL
This page is meant to be used as a reminder after you have gone through waterjet training. 
This page was last updated on 2024-Nov-05

# Access Requirements
To access the waterjet at the AEDL, you must be trained on the waterjet, which requires Ware Lab machine shop certification. If you have WL machine shop certification and would like to be trained to operate the waterjet, talk to your LE.

# Startup Procedure
1. Sign in on the user log clipboard (leave machine hours column blank)
2. Turn off the wall box's breaker switch
3. Inspect the water line to make sure all valves are open (handle inline with pipe)
4. Turn on the machine's main breaker (Located on the side of the machine facing the door)
4. Inspect the pump for water leakage at weap holes. If any water is visible, stop immediately and notify Bob (AEDL manager)
5. Check the level of abrasive media in the feed canister using the stick. If the yellow tape is in the canister, the level of abraisive is low. To load more abrasive, place the sieve over the canister and pour 1 bag of garnet through the sieve to break up any large clusters.
6. Pressurize the garnet feed canister: 1) lift the handle so that the plug closes against the top of the canister, 2) open the valve next to the rim of the canister. Once the valve is open, the pressure will keep the plug in place. CAUTION: if you open the valve before closing the plug, it will spray abrasive media out.
7. On the machine control, press the green "Driver Power" button
8. The machine is now ready for use.

# Shutdown Procedure
1. If in FlowCUT, exit Run Machine mode by clicking the blue return arrow under the Cycle Start button.
2. Close FlowCUT. If popup asks to save changes, do not save changes.
3. Make sure 0.1 inch feeler gauge is back on top of the machine control.
4. Remove workpiece and all workholding from machine table
5. Wash down the table using the hose coiled under the wall mounted electrical box
6. Turn off the machine's main breaker
7. Turn off the wall box's breaker switch 
8. Write down the listed machine hours on the user log clipboard
9. Depressurize the abrasive media pod by closing the valve on the rim. The plug will drop.
10. The machine is now shut down.

# Operation (cutting a part)
0. Follow the Startup Procedure
1. Open FlowPATH software (this is the CAM program for the waterjet)
2. Check the bottom left and confirm that the units are set to the same units the part was designed in
3. Insert a flash drive containing your part .DXF file (**only** DXF files)
4. Load your part through File > Import > (navigate to to your file)
5. (Precaution) Remove undesireable features from the DXF using the Purge button (scissors icon on the right side of the screen)
6. Add tabs through Draw >
7. Generate toolpaths by selecting lines to be cut then clicking the "AP" (auto path) button
8. Confirm that arrows are on the correct sides of the lines.
9. Export as a .ORD file, save in the HPS folder on the desktop.
10. Close FlowPATH. Note: will ask you if oyu want to save changes. Do NOT save changes, because that would overwrite your DXF file.
11. Open FlowCUT from desktop
12. Load your .ORD file
13. In the left pane, select your material from the dropdown (whatever it is, it's almost certainly in there)
14. Enter the material thickness
15. Click the Setup button in the bottom pane. The existing settings are good for >95% of everything, so do not change anything, just hit Confirm.
16. Click the (middle button) in the bottom pane to see a simulation of the machine path. "Watch the cartoon" to completion to confirm the machine will moving as you expect it to.
17. Switch to direct machine control mode by clicking the Run Machine button in the bottom pane (Note: Despite it's name, the "Run Machine" button does not start running the program; only the "Cycle Start" button does that.)
18. Zero the machine axes
19. Jog the head up using PgUp key, and remove the yellow nozzle gaurd, MAKE SURE that the black gasket stays inside the nozzle gaurd. 
20. Load your material onto the table. Generally advisable to secure it with at least 3 clamps. For convenience, can move the machine head away first.
21. Set the Z-height using the 0.1 inch thick feeler gauge on top of the machine control.
22. Look at where your part is in FlowCUT relative to the coordinate origin (bottom left corner), now move the machine head to where that origin should be, such that the actual cuts will be positioned over your material.
23. Set the home position (AKA coordinate origin, AKA G54 offset) for this program: click the house icon in the middle of the jog arrows, select the set home option and confirm.
24. Manually jog the machine head to the corners of the area that will be cut to confirm the head will not collide with any workholding.
25. Set water pump pressure: In FlowCUT, click the green circle under "water pump" to turn on the pump, then walk around to the pump and check the pressure gauge. For all metals -> 55,000 psi, plastics -> 30,000 psi, rubbers and laminates including fiberglass layup -> ~12,000 to 15,000 psi. If needed, adjust the pressure using the black knob on the water pump's housing. WARNING: Do **NOT** exceed 55,000 psi, or go below 12,000 psi; those are the operating limits of the pump.
26. Place the yellow splash guard back on the nozzle, taking care that the black gasket remains fully seated in the guard.
27. Move the machine back to X/Y/Z home position: Click the house icon in the middle of the jog buttons, select the "move to home" option, and confirm. The machine will move back to home. CAUTION: the machine will start the jet at whatever height it is at when you press Cycle Start. It will not automatically move Z back to home position before cutting.
28. If desired, put the polycarb splashgaurds in place (recomended)
29. Start the program by clicking "Cycle Start"
30. (Recomendation) Keep a hand over the spacebar (cycle pause) during first run, just in case anything bad happens.


# Notes and Tips
- In the FlowCUT array tool, the spacings are raw offsets, not any kind of "distance between" measurement 
