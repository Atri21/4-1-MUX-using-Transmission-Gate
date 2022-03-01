# 4-1-MUX-using-Transmission-Gate
# Table of Contents
* [Introduction](https://github.com/Atri21/Design-and-implementation-of-4-1-MUX/blob/main/README.md#introduction)
* [Tools Used](https://github.com/Atri21/Design-and-implementation-of-4-1-MUX/blob/main/README.md#tools-used)
* [Working](https://github.com/Atri21/Design-and-implementation-of-4-1-MUX/blob/main/README.md#working)
* [Netlist](https://github.com/Atri21/Design-and-implementation-of-4-1-MUX/blob/main/README.md#generated-netlist)
* [Acknowledgements](https://github.com/Atri21/Design-and-implementation-of-4-1-MUX/blob/main/README.md#acknowledgements)
* [References](https://github.com/Atri21/Design-and-implementation-of-4-1-MUX/blob/main/README.md#refrences)

# Introduction
The design proposed here is a 4:1 MUX using transmission gate. We implement this using 28nm technology in Synopsis tool. As the MUX we design invloves more inputs, it becomes more complex to build it in traditional way, so designing them using transmission gates is better and in order to fully utilize the power, area and cost advantages of CMOS over SiGe and another semiconductor technology, these circuits must be integrated on one chip. 

# Tools used
* Synopsys Custom Compiler:  The Synopsys Custom Compiler™ design environment is a modern solution for full-custom analog, custom digital, and mixed-signal IC design. As the heart of the Synopsys Custom Design Platform, Custom Compiler provides design entry, simulation management and analysis, and custom layout editing features. This tool was used to design the circuit on a transistor level.
* Synopsys Primewave:  PrimeWave™ Design Environment is a comprehensive and flexible environment for simulation setup and analysis of analog, RF, mixed-signal design, custom-digital and memory designs within the Synopsys Custom Design Platform. This tool helped in various types of simulations of the above designed circuit.
* Synopsys 28nm PDK:  The Synopsys 28nm Process Design Kit(PDK) was used in creation and simulation of the above designed circuit.

# Working
A multiplexer, also known as a data selector, is a device that selects between several analog or digital input signals and forwards the selected input to a single output line. The selection is directed by a separate set of digital inputs known as select lines. The proposed design has 4 input line and 2 select lines and 1 output line.

# Inverter

* Inverter symbol

     ![Screenshot (69)](https://user-images.githubusercontent.com/99316485/156164766-8f53af3d-4932-4f41-b850-9e7c0e233b0e.png)
   
* Inverter design

     ![Screenshot (70)](https://user-images.githubusercontent.com/99316485/156164965-e95902c3-eec2-4b23-8355-a4151d27bcb0.png)

# Tristate 

* Tristate inverter symbol

     ![Screenshot (71)](https://user-images.githubusercontent.com/99316485/156165167-4277f87e-3a3d-4bdc-9499-462a524444cf.png)

* Tristate inverter design

     ![Screenshot (72)](https://user-images.githubusercontent.com/99316485/156165486-3437ad4e-b531-410c-8d80-4efa42cfdf5a.png)

* Tristate inverter truth table

     ![103](https://user-images.githubusercontent.com/99316485/156167512-3ed6e2e2-0087-45aa-9c0a-0bc602af8c80.png)

* Tristate inverter testbench

     ![Screenshot (76)](https://user-images.githubusercontent.com/99316485/156167693-156a1f62-a26b-4b91-9730-a270dea45f95.png)

* Tristate inverter output waveform

     ![Screenshot (77)](https://user-images.githubusercontent.com/99316485/156167842-de515ffc-6705-46f7-bed4-9918351110ea.png)

# Transmission gate

* Transmission gate symbol

     ![Screenshot (78)](https://user-images.githubusercontent.com/99316485/156169374-3505d4dc-5360-4db3-ac9f-93de7203d063.png)

* Transmission gate design

     ![Screenshot (79)](https://user-images.githubusercontent.com/99316485/156169443-6e6e9e97-ee38-45af-b590-82daf3409144.png)

* Transmission gate testbench

     ![Screenshot (80)](https://user-images.githubusercontent.com/99316485/156169661-da21b5f0-1fd2-4a73-a9c3-d46a3f102fb9.png)

* Transmission gate waveform

     ![Screenshot (81)](https://user-images.githubusercontent.com/99316485/156169775-6690ec92-87b5-47e9-9840-866748920ce9.png)

# 4-1 MUX using transmission gate

* 4 : 1 MUX symbol

     ![Screenshot (85)](https://user-images.githubusercontent.com/99316485/156172570-db6f8c67-c49a-4aa4-b64e-1f0afa40a0e2.png)

* MUX Design
    
    ![Screenshot (86)](https://user-images.githubusercontent.com/99316485/156172710-8e01babd-6d32-492a-9b45-63794890d430.png)
    
* MUX Test Bench

    ![Screenshot (87)](https://user-images.githubusercontent.com/99316485/156172814-83535b34-e87e-426c-bc76-d93ffeb810cc.png)
    
* MUX Wavaeform

    ![Screenshot (51)](https://user-images.githubusercontent.com/99316485/156172958-6c96734e-ced5-4669-a4d2-e13a4a92fb3d.png)

## [4-1-MUX-netlist](https://github.com/Atri21/4-1-mux-using-transmission-gate-netlist/blob/main/README.md#4-1-mux-using-transmission-gate-netlist)

# Author
Shiva Kumar S, Sapthagiri College Of Engineering, Bangalore

# Acknowledgements

* Kunal Ghosh, Co-founder, VSD Corp. Pvt. Ltd.
* Synopsys Inc
* IIT Hyderabad
* https://www.iith.ac.in/events/2022/02/15/Cloud-Based-Analog-IC-Design-Hackathon/
* Sameer Durgoji, NIT Karnataka
* Chinmay Panda, IIT Hyderabad

# Refrences 

[1] Wei-Yu Tsai and Ching-Te Chiu “ANovel Low Gate-Count Pipeline Topologywith Multiplexer Flip-Flops for Serial LinkIEEE Transactions on Circuits and Systems:Regular Papers, VOL.59, No. 11, Nov. 2012

[2] M. Alioto and G. Palumbo, “Interconnectawaredesign of fast large fan in CMOSmultiplexers,” IEEE Trans. Circuits Syst. II,Exp. Briefs, vol. 54, no.6, pp. 484-488, Jun2007
