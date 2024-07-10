The N-modular redundant (NMR) system introduces hardware redundancy and fault tolerance by checking that atleast M(<N) modules are functioning as intended.

The triple modular redundancy (TMR) system is the most widely used type of NMR architectures where atleast 2 out of 3 modules are expected to be working as intended and only then will the parent system accept the sub-system's outputs.

![image](https://github.com/anr2311/Fault_Tolerant_Design/assets/72514473/d1d77297-6297-4da0-9c63-3001f0933472)

The same computation/processing is done three times. These modules can be processors, memories, disk drives, buses, network connections, power supplies and so on.

In the simple Simulink model in this repo, there is a triple modular system that introduces offset noise to the incoming input. The voter will then decide if the output produced from the individual sub-systems are equal and produces a boolean output.

If individual reliabilities of each system are known, the following computation can be performed to understand the reliability of the TMR system:

![image](https://github.com/anr2311/Fault_Tolerant_Design/assets/72514473/4c26e74b-9c1e-45f5-8466-5bcc95dca7a9)
