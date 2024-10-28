# Bathymetric Drift Sensor
Low-cost, open-source bathymetric mapping (depth, GPS, angle, datalogging)

Group Members: Autumn, Grant, Teryn, and Camille

This is the repository for the group working on the drifter with GPS, cellular, and bathymetric sensing. We are using a Boron sensor.

Step 1: Find and fork an existing repository to one team member's GitHub account (done), clone (through GitHub desktop) to your computer (done), assess current status, and divide next steps.

Device currently doesn't work well and has not been validated at all. Data is noisy, we need to fix code and maybe update electronics. Noisy because the board requires 5 volts and Boron main output is 3.3 volts. Also using a version of an Adalog measurement, and the quality of that measurement isn't good. The measurement is only as good as the reference to which it is compared, the reference we have is soso but there is a better reference we can use eventually. A big goal will be field validation off the CMS dock. Compare to a groundtruthed measurement like a measuring tape or a fancier sensor to validate our data. 

Goal for 10-28-24: Open premade project folder in VS Code and confirm it will initially compile (compiled successfully). Make sure the cellular is off when running the sensor today. Try flashing the sensor and see what data you get. 

