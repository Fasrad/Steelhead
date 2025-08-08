# Steelhead
Cantilevered cross-gantry 3D printer with unique aesthetics novel features


The belt paths are indexed off the "back" side of the aluminum L. The width of the L doesn't matter as long as it is wide enough to support the rails. 

I've got a lot of questions about the coaxial stepper tower. Such as how the motors are mounted and if it's strong enough. The bottom stepper has a printed washer to make the mounting surface flat, then it's bolted directly to the aluminum L with one screw through the aluminum. The bottom part of the tower screws to the backside of the L, but this connection is not intended to add strength. There are three remaining stepper screws hidden inside the stepper tower that go down and sandwich the L between the stepper tower and stepper; these 3 screws presumably bear the belt tension load of both belts. And then the top stepper is mounted to the top of the tower using through-holes. I recommend keeping the belt tension on the low side. 

The toolhead prints on its side with supports optional. Use a flat or triangle file to clean up the carriage cavities after printing. 

When printing the toolhead, adjust x and Z scale in 0.5% increments to achieve a snug sliding fit to the sides of your carriages. The upper and lower carriages bolt to the lower and upper surfaces respectively, so this doesn't impact the vertical spacing. If vertical spacing needs adjusted, adjust Y scaling in 0.25mm increments. It can be hard to determine if the carriages are too close or too far apart, because the symptoms are similar (binding). Try putting an indicator on the upper one of the cross rails. If it goes down when the toolhead moves towards the unsupported end, the carriage holes are too far apart. You can also use shims...one sheet of copy paper is about 100 microns. A business card is about 400. 
