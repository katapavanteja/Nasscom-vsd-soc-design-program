# nasscom-vsd-soc-design-program
# Contents
 1) [Sky130 Day 1 - Inception of open-source EDA, OpenLANE and Sky130 PDK](https://github.com/katapavanteja/nasscom-vsd-soc-design-program/edit/main/README.md#sky130-day-1---inception-of-open-source-eda-openlane-and-sky130-pdk)
    - [How to talk to computers](https://github.com/katapavanteja/nasscom-vsd-soc-design-program/edit/main/README.md#how-to-talk-to-computers)
       - [Introduction to QFN-48 Package, chip, pads, core, die and IPs](https://github.com/katapavanteja/nasscom-vsd-soc-design-program/edit/main/README.md#introduction-to-qfn-48-package-chip-pads-core-die-and-ips)
       - [Introduction to RISC-V](https://github.com/katapavanteja/nasscom-vsd-soc-design-program/edit/main/README.md#introduction-to-risc-v)
       - [From Software Applications to Hardware](https://github.com/katapavanteja/nasscom-vsd-soc-design-program/edit/main/README.md#from-software-applications-to-hardware)
# Sky130 Day 1 - Inception of open-source EDA, OpenLANE and Sky130 PDK
##  How to talk to computers
###   Introduction to QFN-48 Package, chip, pads, core, die and IPs

**Aurdino Board**: The image below is an Aurdino Microcontroller Board. Here we focus more on the encircled area, which contains the 'Microprocessor',that we will be designing from abstract level till fabrication level by using RTL to GDS flow

![Screenshot 2024-04-25 120653](https://github.com/katapavanteja/nasscom-vsd-soc-design-program/assets/168015988/c8ff1aa9-59fb-4053-a00a-d7378a40045f)

While we cosider the chip, there are 3 main components:

(1) Pads : Through these pads signals can travel into the chip from external sources and viceversa.

(2) Die : It is the whole area of the chip that will be manufactured on the silicon wafer.

(3) Core : It is the area where our entire logic will be implemented.

![Screenshot 2024-04-25 121626](https://github.com/katapavanteja/nasscom-vsd-soc-design-program/assets/168015988/deb72a9c-1f29-4774-9462-1a9475746c8f)

The above mentioned MicroProcessor in an aurdino board is a package that consists of MicroProcessor chip and some other Foundry IP's(Intellectual Property). All of these combined called as a package.

For example, let's consider a package that consists of RISC V SOC and some other IP's such as SRAM , ADC , DAC , PLL etc..

![Screenshot 2024-04-25 122115](https://github.com/katapavanteja/nasscom-vsd-soc-design-program/assets/168015988/3685aa0c-5234-45d8-b8fc-f36cbbdc1dcc)


###  Introduction to RISC-V

**ISA**: ISA is known as "Instruction Set Architecture". It is nothing but a way of communicating with the computer.
In general we write codes that need to be executed by the system, using coding languages like C , Java etc. , but machine can't understand those languages. It is where ISA comes into picture. By using ISA the codes that were written wil be converted into assembly language and from there to binary i.e Machine understandable language. This is the purpose of the ISA, and the RISC V ISA is the latest ISA released.

![Screenshot 2024-04-25 125225](https://github.com/katapavanteja/nasscom-vsd-soc-design-program/assets/168015988/5c651754-2931-4f70-9c35-5b9ef0b5f841)

### From Software Applications to Hardware

In real life we generally deal with Application Softwares(Apps) in order to communicate with the Hardware.But how it's done exactly?
In between Application software and Hardware, there will be a software called System Software. The Applications enter into the System Software and will be converted into the Hardware understandable language i.e Binary Language.
The System Software consists of different layers:
(1) O.S : Other than the general operations like Handling I.O operations, Allocating Memory, Low level System Functions the O.S converts the Application software to respected C,C++,Java etc.. codes.
(2) Compiler : The compiler takes output of O.S as input and converts the codes in C,C++,Java etc.. into Instruction set(.exe files). These instructions will be dependent on type of hardware used.
(3) Assembler : Assembler converts the .exe files into binary language and provides it to the hardware, and hardware performs the respective operations.


