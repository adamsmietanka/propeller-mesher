# Propeller Chart Meshing Tools
Tools used to create fine meshes based on propeller test data. Used by the propeller efficiency calculator.

## Introduction
One of the steps in aircraft design process is calculating the performance figures. 
*Max power, max airspeed* and *max service ceiling* are the most prominent examples. 
In order to calculate them we need to know the engine power and the propeller's **Coefficient of Efficiency *&eta;***. 
An example *&eta;* chart can be seen below:

![Screenshot](docs/images/eff_chart.png)

Where:
  - ***V*** - Aircraft speed
  - ***n*** - Propeller speed
  - ***D*** - Propeller diameter

Designing an aircraft powertrain can be a tedious process when done manually. 
The designer is required to interpolate the data from the chart based on initial conditions in order to calculate the &eta;.
When the user chooses one of the angles from the chart the process is straightforward.
Otherwise the interpolation becomes very time consuming and the precision of the results could be questioned.
The whole process could easily be automated and that led to the development of this application.

## Data source
The application is based on two reports published in 1938 and 1939 respectively by the NASA predecessor - National Advisory Committee for Aeronautics:
  * [NACA 640](http://naca.central.cranfield.ac.uk/reports/1938/naca-report-640.pdf) - Tests of different blade airfoils of propellers having 2, 3 and 4 blades.
  * [NACA 658](http://naca.central.cranfield.ac.uk/reports/1939/naca-report-658.pdf) - Tests of two propellers having at blade angles up to 60°.
