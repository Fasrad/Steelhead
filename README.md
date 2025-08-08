# Steelhead
Cantilevered cross-gantry 3D printer with unique aesthetics novel features


Steelhead is a 3D printer with a unique cantilevered cross-cartesian motion system. It is made of steel, but the name is also inspired by the Steelhead boss in Splatoon.

Parts are printed in regular PLA. Files are included for the laser-cut steel parts as well. Note the steel column is welded and has to have a slot cut out with a saw or cut-off wheel. I also used a lathe to planarize the top after welding.

This is a 1-off, proof-of-concept printer. It is intended to look cool on my desk, but also be a testbed for several ideas which could be adopted or re-purposed on other printers. 

the Steelhead kinematics itself
use of remote electronics box with off-the-shelf DB37 cord
handheld, removable, optional LCD controller
Printed-in-place terminal connections using ring terminals

It's not designed to be easy to build or copy, so don't ask for a kit, or complain that it's hard to assemble.  

I always thought half the value of 3D printing is the entertainment value of watching the machines print. I wanted a small desktop printer with an open design where the print could be seen from many angles, and I didn't want a printer with a moving bed, and I didn't want an enclosed printer like a Voron0. Other
small printers like the Prusa Mini or V-Minion had the “open” aesthetic I wanted, but all of them have moving beds. For this printer, I wanted a small printer with a simplified appearance and no obvious visible electronic components, which did not use a moving bed, and Steelhead is the result.

The Steelhead kinematics are fundamentally the same as cross-gantry kinematics of printers like the Annex K3 or CroXY, but with two motors and two rails deleted. Thus steelhead can be thought of as a cantilevered simplification of the K3 kinematics, in a similar way that the Prusa Mini is a simplification of the Mendel kinematics, with similar compromises. 

Steelhead achieves roughly 150x150x200mm  print volume in a desk space only slightly larger than a Voron 0. Print farms could thus potentially be interested in the potential of these kinematics for space efficiency. It uses a direct-drive extruder with a reverse bowden, but a full bowden version would be possible of course. 

Some technical aspects of Steelhead are deliberately subordinate to the desired aesthetic result, however, it's still a fully functional and usable printer. 

The frame is welded from steel tubing and ¼" mild steel. The single column conceals the Z leadscrew, cable chain, and linear rail all inside, giving a minimalist, utilitarian, and industrial aesthetic. Steel is actually remarkably cheap compared to extrusions. 

The motion gantry is built on a piece of 1/2" MIC6 cast aluminum tool plate, for flatness. The original concept was to use a single square piece of ½ by 8x8 inch tool plate for both the gantry, and the bed. But I decided ½" was too thick for the bed, and ended up using thinner material for the bed, so I didn't get to test that concept. If I had it to do over, I would either try making the gantry out of ¼" aluminum like the bed, and therefore test the concept of making the bed and gantry out of the same piece of aluminum, or I would try building the gantry and/or the bed out of the same 1/4" steel as the rest of the printer. I think for such a small bed, a piece of steel could probably work, but if you made the gantry out of steel, it would definitely have to be surface ground or milled flat after welding. Or maybe leveled with some kind of Moglice. 

The 150mm bed is heated by a 24V, 180W heater. The bed rides on a single MGN9h linear rail and is driven by a concealed leadscrew and motor. The articulating bed mount is stable and easy to level, with independent X and Y tilt adjustments. 

Taking inspiration from the Ratrig V-minion, most electronics are contained off of the printer in a separate electronics case, to keep the printer itself small. However, the V-minion electronics case has a rudimentary umbilical design that limits the potential of the "separate" electronics case. Many people seem to give up on the separate case and set the V-minion on top of the electronics case anyway. I wanted an electronics case that could truly be placed remotely under a desk or something without spoiling the visual effect, so I made a custom case that uses a standard DB37 printer cable. The DB37 cable is the ONLY connection to the printer at all...all power, sensors, stepper wires, and serial cables run through the DB37 cable, and it is long enough to place the electronics case under the desk, and also convenient to connect and disconnect for transport.  

The reverse bowden system pulls filament upward. So steelhead can either pull from a spool placed on rollers, or it can pull filament up from a filament box placed below the desk. 

I initially wanted to build the printer with no LCD screen, and have a dedicated control panel on the printer with tactile buttons and switches. However, making such a control panel would be a project as big as the printer itself, so that is left as a future project. I still wanted the option to remove the LCD controller, so the controller is connected to the printer with a coiled tether. With the coiled cord, it can be handheld like a videogame controller or a control pendant. This is very convenient when making printer adjustments. But if you want to run the printer without the LCD controller, you can simply unplug the LCD altogether and run the printer by wifi or USB. The LCD controller docks to the printer with magnets when not in use.  

Technical/build notes 

The belt paths are indexed off the "back" side of the aluminum L. The width of the L doesn't matter as long as it is wide enough to support the rails. 

I've got a lot of questions about the coaxial stepper tower. Such as how the motors are mounted and if it's strong enough. The bottom stepper has a printed washer to make the mounting surface flat, then it's bolted directly to the aluminum L with one screw through the aluminum. The bottom part of the tower screws to the backside of the L, but this connection is not intended to add strength. There are three remaining stepper screws hidden inside the stepper tower that go down and sandwich the L between the stepper tower and stepper; these 3 screws presumably bear the belt tension load of both belts. And then the top stepper is mounted to the top of the tower using through-holes. I recommend keeping the belt tension on the low side. 

The toolhead prints on its side with supports optional. Use a flat or triangle file to clean up the carriage cavities after printing. 

When printing the toolhead, adjust x and Z scale in 0.5% increments to achieve a snug sliding fit to the sides of your carriages. The upper and lower carriages bolt to the lower and upper surfaces respectively, so this doesn't impact the vertical spacing. If vertical spacing needs adjusted, adjust Y scaling in 0.25mm increments. It can be hard to determine if the carriages are too close or too far apart, because the symptoms are similar (binding). Try putting an indicator on the upper one of the cross rails. If it goes down when the toolhead moves towards the unsupported end, the carriage holes are too far apart. You can also use shims...one sheet of copy paper is about 100 microns. A business card is about 400. 
