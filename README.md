# VLSI-CMOS-Inverter-DesignFlow
A complete VLSI design flow for a CMOS inverter using Cadence Virtuoso. Covers schematic design, symbol creation, testbench setup, transient and DC analysis, layout generation, DRC and LVS checks. AV extraction is pending. Ideal for students and professionals in VLSI design.
The project demonstrates a full design flow for a CMOS inverter, a fundamental building block in VLSI design. Using Cadence Virtuoso, the following steps are covered:
1. Schematic Design: A well-structured CMOS inverter schematic.
2. Symbol Creation: A reusable symbol for hierarchical design.
3. Testbench Setup: Configuring testbenches for transient and DC simulations.
4. Transient and DC Analysis: Detailed simulation results, ensuring the design meets performance criteria.
5. Layout Generation: Converting the schematic to a physical layout while adhering to design rules.
6. DRC and LVS Checks: Ensuring that the layout is error-free and matches the schematic design.
7. AV Extraction (Pending): The final step, parasitic extraction, will be added shortly.

Lets Start
1. Schematic Design:
 <br>
The schematic design represents the initial step in developing the CMOS inverter. It shows the electrical connections and components that make up the circuit, which is crucial for understanding the circuit’s functionality and design.

The CMOS inverter schematic includes the following key components:
- PMOS and NMOS transistors: These transistors are the core of the CMOS inverter circuit.
- Power supply: Provides the necessary voltage for the circuit to operate.
- Input and output: The input signal is processed by the inverter to produce the output signal.

The schematic diagram illustrates how these components are connected to achieve the desired inverter functionality.

Below is the schematic diagram of the CMOS inverter:

![Inverter Schematic Design](https://github.com/user-attachments/assets/13bcb6cb-bb7d-42ca-b338-42173e372ea6)

This schematic provides a detailed view of the CMOS inverter’s design and is essential for the subsequent steps, such as Testbench, simulation and layout design. Understanding the schematic helps ensure that the circuit performs as expected.

2. Symbol creation:
<br>
Symbol creation involves designing a graphical representation of the CMOS inverter that will be used in schematic diagrams. This symbol simplifies the representation of the inverter in circuit designs and helps in maintaining a clear and organized schematic layout.

The symbol for the CMOS inverter includes:
- Pin configuration: Labels for input and output pins are clearly marked.
- Visual representation:The symbol is designed to visually represent the CMOS inverter in a compact and recognizable format.
- Standardized layout:The symbol follows standard conventions for consistency in schematic diagrams.

The symbol is used in schematic diagrams to easily incorporate the CMOS inverter into larger circuit designs.
Below is the symbol created for the CMOS inverter:

![Inverter Symbol Creation](https://github.com/user-attachments/assets/8072a8d7-0578-4740-bad3-ad4b7a9cd3a0)

Creating the symbol for the CMOS inverter is essential for integrating the inverter into schematic diagrams. It provides a standardized way to represent the inverter, making the design process more efficient and organized.

3.Testbench Setup
<br>
The testbench setup for the CMOS inverter involves configuring input and power signals to verify the circuit's functionality. This section describes the connections and components used in the testbench.

The testbench setup consists of the following components:

- Pulse Source (VPULSE): Provides a pulsed signal to the input of the CMOS inverter. This simulates varying input conditions to test the inverter’s response.
- DC Voltage Source (VDC): Provides a constant DC voltage to power the CMOS inverter. It is connected to the VDD and VSS pins of the inverter.
<br>
Connections:
  - VPULSE Connection: Connect the output of the VPULSE source to the input pin of the CMOS inverter, This applies the pulsed input signal.
  - VDC Connection: Connect the positive terminal of the VDC source to the VDD pin of the CMOS inverter and the negative terminal to the ground. This supplies power to the inverter.
  - Output Monitoring: Connect the output pin of the CMOS inverter to an observation tool or probe to monitor the output signal.

Below is the diagram of the testbench setup for the CMOS inverter:

![Inverter Testbench Creation](https://github.com/user-attachments/assets/682f2699-bf14-4a03-a028-092f4b4b56ca)

The testbench setup for the CMOS inverter uses a pulse source (VPULSE) to apply varying input signals and a DC voltage source (VDC) to power the circuit. By connecting these sources to the appropriate pins and monitoring the output, the testbench helps verify the inverter’s functionality and performance.

4. Transient Analysis

Transient analysis is used to observe the time-varying behavior of the CMOS inverter. This analysis shows how the inverter responds to changes in input signals over time.

1. Setup Transient Analysis:
   - Set the Stop Time to 200 nanoseconds.
   - Choose Moderate Mode for the simulation.

2. DC Analysis Setup:
   - Select the option to Save DC Operating Point.
   - Choose Component Parameter for the sweep type.
   - Select VPULSE as the component for DC sweep.
   - Set the sweep range from 0 to 1.8 volts.

Below are the results from the transient analysis:


<img width="665" alt="ADE L " src="https://github.com/user-attachments/assets/139d9c44-c0fe-44bb-b6b4-984b75c3290b">


3. Plotting Results:
   - Select Output and Input lines for plotting.
   - Run the transient analysis and review the results.

4. Netlist and Simulation:
   - Ensure the netlist is generated correctly.
   - Execute the simulation to analyze the transient response of the CMOS inverter.


1. Result of Transient Response
   

     <img width="960" alt="Transient Response" src="https://github.com/user-attachments/assets/232af5dc-bd4c-4461-a2e0-eef39599e3a5">


3. Result of DC Output without input
   
     
<img width="960" alt="DC output 1" src="https://github.com/user-attachments/assets/2ffb0f08-b749-4519-abd0-58307edf6695">


3. Result of DC Output with input
   
   
     <img width="960" alt="DC Output 2 with Input" src="https://github.com/user-attachments/assets/7be60c78-706e-41d2-83d2-9162d5aa06cd">


5. Result of Output Current
   

<img width="960" alt="Current Plot" src="https://github.com/user-attachments/assets/ce9246b2-1580-4a6d-b51f-2a647f4505d2">


5.  Result of both DC and Current Output
   

     ![DC with Current Output](https://github.com/user-attachments/assets/055ef255-fa2e-49bd-91db-b18a804fab99)



7. Final Result
   

     ![Final Result](https://github.com/user-attachments/assets/7f4e3a6a-c6a9-4d6c-83a8-31c3c3aea1d8)


- 5. Layout Generation : DRC and LVS Checked

DRC Checked

![Inverter Layout with DRC Check](https://github.com/user-attachments/assets/7ffce0f4-4f2f-46d0-8bea-a0283ec9d05d)


The image above presents the results of the Design Rule Check (DRC) for the CMOS inverter layout. The check has been successfully completed with no violations detected, as indicated by the absence of any error highlights. This confirms that the layout adheres to all design rules and is fully compliant, allowing it to proceed to the next stages in the design flow.


LVS Checked

first image 

![Inverter Layout with LVS](https://github.com/user-attachments/assets/9044d869-7a92-41eb-b818-2a1d83731bb0)


second image

![Schematic and Layout Match](https://github.com/user-attachments/assets/7a960ef0-a3e1-49de-bc2b-aaf14e00376b)

The image above shows the results of the Layout Versus Schematic (LVS) check for the CMOS inverter. The LVS check confirms a complete match between the layout and the schematic, with no discrepancies identified. This result verifies that the layout accurately represents the schematic design and is error-free.


     



