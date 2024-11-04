# Bathymetric Drift Sensor
Low-cost, open-source bathymetric mapping (depth, GPS, angle, datalogging)

Group Members: Autumn, Grant, Teryn, and Camille

This is the repository for the group working on the drifter with GPS, cellular, and bathymetric sensing. We are using a Boron sensor.

Step 1: Find and fork an existing repository to one team member's GitHub account (done), clone (through GitHub desktop) to your computer (done), assess current status, and divide next steps.

Device currently doesn't work well and has not been validated at all. Data is noisy, we need to fix code and maybe update electronics. Noisy because the board requires 5 volts and Boron main output is 3.3 volts. Also using a version of an Adalog measurement, and the quality of that measurement isn't good. The measurement is only as good as the reference to which it is compared, the reference we have is soso but there is a better reference we can use eventually. A big goal will be field validation off the CMS dock. Compare to a groundtruthed measurement like a measuring tape or a fancier sensor to validate our data. 

10-28-24 Goals: Open premade project folder in VS Code and confirm it will initially compile (compiled successfully). Make sure the cellular data is off when running the sensor today (attempted). Try flashing the sensor and see what data you get (unable to attempt). 

11-4-24 Goals: Try flashing the sensor and see what data you get. Determine the buoyancy of the drifter, replace the PVC pipes that are cracked, glue the PVC pipes together more securely, stabilize the drifter. Replace the older electronics with newer versions?

