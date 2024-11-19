## Ex No: 03     Implementation & Analysis of D-flipflop using Cadence EDA Tools   

## Aim:
To design and implement a D-flip-flop using Cadence EDA tools, simulate its behavior, and analyze key performance parameters such as timing, power consumption, and resource utilization for a comprehensive understanding of sequential logic circuits.

## Tools Required:
  - Personal Computer
  - Cadence Virtuoso Software

## Circuit Diagram:

![IMG-20241115-WA0008](https://github.com/user-attachments/assets/e21d408b-0416-437d-81e0-e5781a11717d)



### SCHEMATIC SIMULATION:
PROCEDURE FOR CREATING THE SCHEMATIC SIMULATION
Commands to get into Cadence:

1. Right-click and open the terminal window.
2. Type the following commands and press enter
    - csh
    - source /cadence/install/cshrc
    - virtuoso
    
Procedure for Schematic simulation using Cadence

1) Now two windows must open
  i)virtuoso/command interpreter window ii)”Whats New…”

2) Close the 2nd window
 
 
3) Use 1st window i.e virtuoso window(CIW) for further processing.
    - Create a New Library
    - Create Schematic Cell view.
    - Create the Symbol for schematic Cell view.
    - Create the test Cell view.
    - Analog simulation by spectre

### Steps for Schematic Simulation using Cadence:
i) Procedure for Creating a New Library:
  - File → New → Library
  - Name the library (e.g., VLSILAB_EXP_3).
  - Choose "Attach to an existing technology library" and click OK.
  - Attach the library to the technology library gpdk045. Click OK.
    
ii) Create Schematic Cell View:
 In the Virtuoso (CIW) window:
  - Go to 1st window i.e virtuoso(CIW)
  - File-New-Cell view
  - Setup the new file form
       + Library: Select the one you a created.
       + Cell : Give the experiment name Ex: Inverter View_Schematic
       + Type: Schematic press OK

   - Add the required components from the libraries and make the connections.
       + Go to instance fixed menu or use shortcut key “I” from keypad to go instances
       + Click on browse. This opens the library browser
       + Now select the appropriate library for components like
       + Gpdk45 ------------------------nmos1v, pmos1v
       + Create Input and Output pins
       + Make the connections by using fixed narrow wire key
       + Click Check and Save button
    
         
![Screenshot 2024-10-19 175851](https://github.com/user-attachments/assets/43a8f8c6-26a2-4f57-86f9-fb048adb7260)




 
iii)	Creating the Symbol for schematic Cell view

   - In the schematic window, execute
       + Create – Cell view – From Cell view
       + The cell view from cell view window appears
       + Check Lib Name, Cell Name, From View name must be schematic Press ok
   - Now Symbol generation form appears. Click Ok If No changes required
   - A new window with with default symbol is created.
   - Edit the symbol if you want to give actual symbol shape else continue.
   - Execute Create-Cell view-from cell view
   - Library Name and Cell Name must be same which you have used for schematic. Press OK
   - Check for the position of pin side.Prss OK
   - Edit for the shape by Create-Shape-Choose required options to edit.


![Screenshot 2024-10-19 180009](https://github.com/user-attachments/assets/bf8d1f12-4ec2-4ffa-bbbe-86db56a24db0)



### iv) Creating the Test Cell View:
- In the CIW window:
  + File → New → Cell view
- In the new file form, set the following:
   + Library: Select the library you created earlier (e.g., VLSILAB_EXP_3).
   + Cell: Name it something different from the schematic cell (e.g., DFlipFlop_test).
   + View: Select "Schematic."
   + Type: Schematic. Press OK.
- Add the required components and make connections, similar to step ii.

![Screenshot 2024-10-19 181931](https://github.com/user-attachments/assets/37981a8d-18db-421d-ae28-832f55a93615)



 
### Analog Simulation by SPECTRE:

   - In test cell view window
   - Launch – ADE L(Analog Design Environment)
       + Execute Setup—Simulation/directory/Host A new window opens
       + Set the simulation window to spectre and click ok
       + Execute Analysis – Choose. A window opens.
       + Select the type and set the specifications and press OK
       + Execute Output s—to be plotted – Select on Schematic
       + Then Select the INPUT WIRE(Vin ) and OUTPUT WIRE(Vout) from your test Schematic using mouse
   - Execute Simulation -- Net list and Run
 
![Screenshot 2024-10-19 182155](https://github.com/user-attachments/assets/55eee15d-65e8-47ca-a4f5-7e19f2aed6e7)



## For Transient Analysis Settings and Output
- In the simulation setup, choose transient analysis.
  - Specify the time range for the analysis (start and stop time).
  - Run the simulation and observe the output waveforms for the D and Q signals.

 
![Screenshot 2024-10-19 182209](https://github.com/user-attachments/assets/ac42e513-b6c8-4c78-9242-3f5ec15152a7)


![Screenshot 2024-10-19 183235](https://github.com/user-attachments/assets/7e72c054-cdcc-46d4-98a9-3167ff21626c)



## Results:
The design and implementation of the D-flip-flop using Cadence EDA tools were successfully completed. The simulated results confirmed the correct operation of the flip-flop, with proper synchronization of the input data with the clock signal. Key performance parameters such as propagation delay, power consumption, and area utilization were evaluated, aligning with expected theoretical values.











