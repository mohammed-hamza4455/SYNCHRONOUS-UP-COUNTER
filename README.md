# EXP:11: SYNCHRONOUS UP COUNTER
## NAME:MOHAMMED HAMZA
## REG NO:24900511

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

/* write all the steps invloved */

**PROGRAM**

![EXP 11 CODE](https://github.com/user-attachments/assets/9d04421e-2f4a-471f-94e5-71399fbcdf5d)



**TRUTH TABLE**
![EXP 11 TRUTH](https://github.com/user-attachments/assets/2f59de09-1f03-4b40-9832-1f11b0ad5e4a)

**RTL LOGIC**
![EXP 11 RTL](https://github.com/user-attachments/assets/f8747c62-7912-47ed-ade6-e18dd1fb7f65)
**RTL OUTPUT**
![EXP 11 RTL OUTPUT](https://github.com/user-attachments/assets/fd2b4104-f2ba-451b-8f03-f7a1e46f3e95)

**RESULT**
Thus we have to implement 4 bit synchronous up counter and validate functionality.
