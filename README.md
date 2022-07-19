# Data-analysis
AIM:

 To write a python program which reads the engine output parameter data file and perform the required objectives.




**OBJECTIVES:**

To calculate the area under the P-V diagram. P is in column 2 and V is in column 8.
To calculate the power output of this engine. Assuming that the RPM is 1500.
To calculate its specific fuel consumption.

**PROBLEM STATEMENT:**

We have to calculate the basic performance calculation engine and plot graph by following the conditions given below:

 The code should take column numbers as the input and plot the respective columns as separate images and each file should be saved by the name of the column
The plot labels should be extracted from the file and the label information should automatically be extracted and must appear as labels in the plots. 
The code should exit gracefully, if a non-compatible file is provided as an input. It should say  "File not recognized. Please provide a valid CONVERGE output file".

**SOLUTION PROCEDURE:**

Firstlt, the required modules are imported . Modules like

  'matplotlib.pyplot': for ploting graphs

  'sys' : for system exit

  'numpy' : for array

  'simps' : to find area under curve

Then compatability check is made, that is to check whether the input of specified coverge file is  correct or not, if it is correct program will be exicuted else the program will throw a error saying that "File not recognised.Please provide a valid converge output file" 
Then data is visualised , Once the data is read, the code will ask two input i.e. 2 column numbers of the engine parameters to show its characteristics. If the column number exeeds the range the program will not run and i will exit from the code.
If the correct column numbers of the engine parameter is entered then the code will be successfully be executed.It will read the file , extracts the required parameter name and units, extracts parameter values and store those values and plots the graph between the parameter with their names as labels of the corresponding axis.
In order to calculate the basic performance of the engine we have to give a of (2 8) as they both refers to the pressure and volume column
The area under the curve is calculated using 'simps'(simpson rule) and the area under the curve gives the workdone by the engine.
The obtained area is used to calculate the power output of the engine and the obtained power output is used to calculate the specific fuel consumption.
The code will perform the basic calculation only when the input column values correspond to the volume and pressure respectively.






**OUTPUT:**

COMPATIBILITY TEST:<br /> 
![1](https://user-images.githubusercontent.com/104487026/179746803-88657953-6bbb-4974-b709-a05715481eb8.png)<br />

PLOTTING PRESSURE VS CRANK:
![2](https://user-images.githubusercontent.com/104487026/179746908-1510f57e-9e55-473f-a7cb-ef3434952156.png)<br />
![3](https://user-images.githubusercontent.com/104487026/179746940-7f46dafa-03e9-4c40-92e1-fa312d6eca60.png)<br />


PLOTTING MEAN TEMPERATURE VS CRANK:<br />
![4](https://user-images.githubusercontent.com/104487026/179747032-0c2d24cb-479d-4a3c-ab7d-30c6b8fe0bc1.png)<br />
![5](https://user-images.githubusercontent.com/104487026/179747070-fbbb584a-0edb-4dbf-9b89-87f05b577946.png)<br />


PLOTTING VOLUME VS CRANK:<br />

![6](https://user-images.githubusercontent.com/104487026/179747203-c79cd807-34d3-4469-a8b2-9ab87e74272b.png)<br />
![7](https://user-images.githubusercontent.com/104487026/179747233-4b54df51-0693-46a6-846c-0be4c118ec1f.png)<br />




 **BASIC PERFORMANCE:**<br />
![8](https://user-images.githubusercontent.com/104487026/179747363-45425407-4cb5-413c-827e-752a028b4dca.png)<br />
![9](https://user-images.githubusercontent.com/104487026/179747389-d8225c07-c264-48bc-b10d-39c44f136587.png)<br />


 
