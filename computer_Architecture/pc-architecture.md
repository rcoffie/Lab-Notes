
# Basic Computer Hardware Architecture

A computer hardware Architecture is the science and art of designing computer platforms (hardware, system, sw and programming model) to archive as set of goals.

**Note**
designing a super computer is different from designing a smartphone but many Fundamentals and principles are similar.

### Previous Computer CPU Design
## Previous PC Architecture

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)

previously  computer CPU (Central Processing Unit) was connected to component on the motherboard indirectly.\
The central  processing unit **(CPU)** include an Arithmetic Logical Unit **(ALCU)**
, Control Unit **CU** and Registers.

The CPU was connected to a chip on the mother board knows as the north bridge memory controller, this settings is via a front side bus. the north bridge is connected to the DRAM dynamic random access ram via a memory bus. 

The north bridge connects to the Graphics adopter via PCI. Express adopter also known as Peripheral component interconnect express. 
with this most time the north bridge is been referred to us the graphics controller hub.
The North bridge was also connected with the south-bridge via DMI. direct media interface bus.

The south bridge was connected to the slow devices such as the input and output devices, keyboard and mouse , hard drive controller , network devices ,USB port etc, for this reason the south bridge was been fe to as the input out put controller.

The north bridge and the south bridge were collectively referred to as the chipset.


## The Modern PC Architecture

![App Screenshot](https://via.placeholder.com/468x300?text=App+Screenshot+Here)

The modern CPU of a PC is likely to have multiple physical core, at least a modern day pc has two cores but can go up from four to eight and more.
Each core has it own ALU, Control Unit and it own sets or registers . Each core is cable of executing a program instruction independently . most modern software are guild to make use of multiple  cores this increase performance.

Modern CPU's has a large amount of high speed level of cache memory, in the modern architecture the north bridge no longer exists. the memory and graphics controller are now integrated into the CPU chip. this remove the need for a front side bus between the cpu and the ram . this has had a huge impact on the performance on the modern PC.

The south bridge is been replaced by a chipset. this works as hub to control the slower devices, like mouse and keyboard, usb input and output devices , network adapter ext.
The chipset is connected to the CPU via a high speed bus call the DMI.

The mother board also has a crystal oscillator on it . A crystal oscillator is an electronic oscillator that makes use of piezoelectric effect. it makes use of the mechanical resonance of the vibrating crystal, which has piezoelectric properties, in order to obtain an electric signal with a high-precision frequency. Crystal oscillator are considered superior to ceramic resonators as they have higher stability, higher quality , lower cost and smaller in size .
The base clock frequency is 100 MHZ 

Cache Memory is the temporary memory. this chip-based feature of your computer lets you access some information more quickly than if you access if from your computer main hard drive.
Cache memory are often referred to as SRAM (Static RAM) is a type of Random Access Memory (RAM) that retains data bit in it's memory as long as power being supplied.

DRAM. 
Dynamic random access memory (DRAM) is a type of semiconductor memory that is typically used for the data or program code needed by a computer processor to function. DRAM  is a common type of random access memory (RAM) used in personal computers (PC's). Workstations and Servers.

RAM is part of the computers Main Memory, which is directly accessible by the CPU. Radom access allows the PC processor to directly access any part of the memory rather than proceeding sequentially from a starting place . RAM is located close to a computer processor and enable faster access to data than storage media such as hard disk drives and solid stated drives . RAM is used to store data that is currently is currently processed by the CPU. Most of the programs and data that are modifiable are stored in the RAM. Integrated RAM chips are available in two forms. 

SRAM (STATIC RAM)
DRAM (DYNAMIC RAM)

Dynamic random access memory stores each bit of data in a separate capacitor within and integrated circuit. The charging and discharging of the capacitor represent 0 and 1 , example the to possible values can be stored in a bit. 

DRAM is widely used in digital electronic where low-cost and high capacity memory is required 
