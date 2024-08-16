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
1. Schematic Design
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
2. Symbol creation

Symbol creation involves designing a graphical representation of the CMOS inverter that will be used in schematic diagrams. This symbol simplifies the representation of the inverter in circuit designs and helps in maintaining a clear and organized schematic layout.

The symbol for the CMOS inverter includes:
- Pin configuration: Labels for input and output pins are clearly marked.
- Visual representation: The symbol is designed to visually represent the CMOS inverter in a compact and recognizable format.
- Standardized layout: The symbol follows standard conventions for consistency in schematic diagrams.

The symbol is used in schematic diagrams to easily incorporate the CMOS inverter into larger circuit designs.
Below is the symbol created for the CMOS inverter:

![Inverter Symbol Creation](https://github.com/user-attachments/assets/8072a8d7-0578-4740-bad3-ad4b7a9cd3a0)

Creating the symbol for the CMOS inverter is essential for integrating the inverter into schematic diagrams. It provides a standardized way to represent the inverter, making the design process more efficient and organized.

3.Testbench Setup

The testbench setup for the CMOS inverter involves configuring input and power signals to verify the circuit's functionality. This section describes the connections and components used in the testbench.

The testbench setup consists of the following components:

- Pulse Source (VPULSE): Provides a pulsed signal to the input of the CMOS inverter. This simulates varying input conditions to test the inverter’s response.
- DC Voltage Source (VDC): Provides a constant DC voltage to power the CMOS inverter. It is connected to the VDD and VSS pins of the inverter.
- *Connections*:
  - VPULSE Connection: Connect the output of the VPULSE source to the input pin of the CMOS inverter. This applies the pulsed input signal.
  - VDC Connection: Connect the positive terminal of the VDC source to the VDD pin of the CMOS inverter and the negative terminal to the VSS pin (ground). This supplies power to the inverter.
  - Output Monitoring: Connect the output pin of the CMOS inverter to an observation tool or probe to monitor the output signal.

Below is the diagram of the testbench setup for the CMOS inverter:

![Inverter Testbench Creation](https://github.com/user-attachments/assets/682f2699-bf14-4a03-a028-092f4b4b56ca)

The testbench setup for the CMOS inverter uses a pulse source (VPULSE) to apply varying input signals and a DC voltage source (VDC) to power the circuit. By connecting these sources to the appropriate pins and monitoring the output, the testbench helps verify the inverter’s functionality and performance.
