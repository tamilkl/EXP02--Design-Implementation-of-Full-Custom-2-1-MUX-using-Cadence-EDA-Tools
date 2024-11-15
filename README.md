# EXP02--Design-Implementation-of-Full-Custom-2-1-MUX-using-Cadence-EDA-Tools##
### Aim:
To design and implement a 2:1 multiplexer (MUX) circuit using Cadence EDA tools, analyse its functionality and performance, and understand the principles of digital logic design, including schematic creation, layout design, and simulation.
### Tools Required:
•	Personal Computer<br>
•	Cadence Virtuoso Software<br>

### S C H E M A T I C S I M U L A T I O N
### PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION
### Commands to get into Cadence
1.	Right Click and open the terminal window<br>
2.	Type the following commands as follows and press enter.<br>
•	csh<br>
•	source /cadence/install/cshrc<br>
•	virtuoso <br>
### Procedure for Schematic simulation using Cadence

1.	Now two windows must open<br> i)virtuoso/command interpreter window<br> ii)”Whats New…”<br>
2.	Close the 2nd window
3.	Use 1st window i.e virtuoso window(CIW) for further processing.<br>
i.	Create a New Library<br>
ii.	Create Schematic Cell view.<br>
iii.	Create the Symbol for schematic Cell view.<br>
iv.	Create the test Cell view.<br>
v.	Analog simulation by spectre<br>


### i)	Procedure for Creating New Library.
•	File –New – Library<br>
•	Name : Give name for ur library Ex: VLSILAB_EXP_1<br>
•	Enable Attach to an existing technology library, Click OK<br>
•	Attach the library to the technology library gpdk045.Click OK<br>
### ii)	Create Schematic Cell view.
•	Go to 1st window i.e virtuoso(CIW)<br>
•	File-New-Cell view<br>
•	Setup the new file form<br>
	  Library: Select the one you a created.<br>
	  Cell : Give the experiment name Ex: Inverter View_Schematic<br>
	  Type: Schematic press OK<br>
•	Add the required components from the libraries and make the connections.<br>
	Go to instance fixed menu or use shortcut key “I” from keypad to go instances<br>
	Click on browse. This opens the library browser<br>
	Now select the appropriate library for components like 
	Gpdk45 ------------------------nmos1v,  pmos1v<br>
	Create Input and Output pins<br>
	Make the connections by using fixed narrow wire key<br>
	Click Check and Save button<br>
![image](https://github.com/user-attachments/assets/49501ed9-e987-4181-b8a2-777243222ce5)



 
### iii)	Creating the Symbol for schematic Cell view<br>
•	In the schematic window, execute <br>
	Create – Cell view – From Cell view<br>
	The cell view from cell view window appears<br>
	Check Lib Name, Cell Name, From View name must be schematic Press ok<br>
•	Now Symbol generation form appears. Click Ok If No changes required<br>
•	A new window with with default symbol is created.<br>
•	Edit the symbol if you want to give actual symbol shape else continue.<br>
•	Execute Create-Cell view-from cell view<br>
•	Library Name and Cell Name must be same which you have used for schematic. Press OK<br>
•	Check for the position of pin side.Prss OK<br>
•	Edit for the shape by Create-Shape-Choose required options to edit.<br>

 ![image](https://github.com/user-attachments/assets/46b1c0de-d01e-43aa-9ab6-479623749b8e)




### iv)	Creating the new test cell view<br>
•	Go to CIW window, Execute File-New-Cell view<br>
	Setup the new file form<br>
	Library: Select the one you created.<br>
	Cell: Cell name must be different from the name used in schematic cell view. Ex: Inverter_test<br>
	View: Schematic<br>
	Type: Schematic press OK<br>
•	Follow the step 3(ii) d to make the required connections<br>
![image](https://github.com/user-attachments/assets/ed3ed107-6de4-4ccf-b1d1-fc478acb493a)



### Analog simulation by SPECTRE.<br>
•	In test cell view window<br>
•	Launch – ADE L(Analog Design Environment)<br>
	Execute Setup—Simulation/directory/Host A new window opens<br>
	Set the simulation window to spectre and click ok<br>
	Execute Analysis – Choose. A window opens.<br>
	Select the type and set the specifications and press OK<br>
	Execute Output s—to be plotted – Select on Schematic<br>
	Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse<br>
•	Execute Simulation -- Net list and Run<br>
![image](https://github.com/user-attachments/assets/664de7e1-ba8f-4b00-8fd2-3b584ede7a4f)


For Transient Analysis Settings and Output
![image](https://github.com/user-attachments/assets/0ff69da9-5643-4f4a-86ad-e64ff91f1900)


![image](https://github.com/user-attachments/assets/f828b33b-6b0c-4220-9fb4-85b18d6655cc)



 

### Results:<br>
1.	The experiment successfully demonstrated the design and implementation of a 2:1 MUX using Cadence EDA tools.<br>
2.	The successful verification through schematic, layout, and simulation underscores the effectiveness of using Cadence EDA tools for digital circuit design.
