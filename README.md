# EXP:11: SYNCHRONOUS UP COUNTER
## NAME:MOHAMMED HAMZA
## reg no:24900511

**AIM:**

To implement 4 bit synchronous up counter and validate functionality.

**SOFTWARE REQUIRED:**

Quartus prime

**THEORY**

**4 bit synchronous UP Counter**

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/d5db3fa0-e413-404c-b80e-b2f39d82e7e8)


![image](https://github.com/naavaneetha/SYNCHRONOUS-UP-COUNTER/assets/154305477/52cb61eb-d04b-442d-810c-31185a68410b)

Each flip-flop in this circuit will be clocked at exactly the same time.
The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.”
Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse.
Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time.
The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed.
However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

**Procedure**
1.Type the program in Quartus software.

2.Compile and run the program.

3.Generate the RTL schematic and save the logic diagram.

4.Create nodes for inputs and outputs to generate the timing diagram.

5.For different input combinations generate the timing diagram.


**PROGRAM**
![EXP 11 CODE](https://github.com/user-attachments/assets/00f0bc81-7d59-41c0-a723-64f4dea79049)

**TRUTH TABLE**
![EXP 11 TRUTH](https://github.com/user-attachments/assets/f7c0c837-255d-49f5-a554-fe5e9012a0c8)

**RTL LOGIC**
![EXP 11 RTL](https://github.com/user-attachments/assets/6832cb3b-02db-455e-9034-e014db1a2085)


**RTL OUTPUT**
![EXP 11 RTL OUTPUT](https://github.com/user-attachments/assets/9afd87fe-a0c9-478c-a12c-ee26cdd5c646)




**RESULTS**
Thus we have implemented and verified 4 bit synchronous up counter and validate functionality
