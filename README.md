# Automatic-Transmission
A model of Automatic Transmission made using OpenSCAD

It has six forward speeds and one reverse. Real automatic transmissions have a hydraulic or electrical system that engages different clutches and brakes to shift gears depending on the driving situation. With this model you control those simplified brakes and clutches yourself.
The clutch is actuated by sliding the drive shaft through to different positions (which each have two gear markings), while three separate brakes each also have two gear markings. You select a gear by engaging the brake and clutch position associated with your desired gear.
I tried to design the gear ratios to be fairly close to what some real cars use, and this is the result, where the input is the crank and the output is the annulus:
1st gear: 1 : 4.29
2nd gear: 1 : 2.5, 71% increase
3rd gear: 1 : 1.67, 50% increase
4th gear: 1 : 1.3, 28% increase
5th gear: 1 : 1, 30% increase
6th gear: 1 : 0.8, 25% increase
Reverse: 1 : -3.93
The OpenSCAD file is included and is highly parametric in case you'd like to play with different gear ratios. If you select a different number of teeth, it will print out the resulting gear ratios at the beginning of the output. I also used MATLAB to investigate more thoroughly how the gear sizes affected the various ratios. I used transmission.m as an aid in optimizing the ratios to be somewhat evenly spaced.

Thanks to FreeCAD and OpenSCAD community and documentation. The entire project is just a product of tutorials provided by the respective communities.
