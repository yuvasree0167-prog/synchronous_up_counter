# synchronous_up_counter
AIM:

To implement 4 bit synchronous up counter and validate functionality.

SOFTWARE REQUIRED:

Quartus prime

THEORY

4 bit synchronous UP Counter

If we enable each J-K flip-flop to toggle based on whether or not all preceding flip-flop outputs (Q) are “high,” we can obtain the same counting sequence as the asynchronous circuit without the ripple effect, since each flip-flop in this circuit will be clocked at exactly the same time:

<img width="594" height="321" alt="Screenshot 2025-12-15 175535" src="https://github.com/user-attachments/assets/08ff7dae-36cc-4cc7-8c5f-b4ce0c093ba2" />



<img width="811" height="424" alt="Screenshot 2025-12-15 175546" src="https://github.com/user-attachments/assets/ae48c48c-eadd-4e48-a004-f3d81e99fa27" />


Each flip-flop in this circuit will be clocked at exactly the same time. The result is a four-bit synchronous “up” counter. Each of the higher-order flip-flops are made ready to toggle (both J and K inputs “high”) if the Q outputs of all previous flip-flops are “high.” Otherwise, the J and K inputs for that flip-flop will both be “low,” placing it into the “latch” mode where it will maintain its present output state at the next clock pulse. Since the first (LSB) flip-flop needs to toggle at every clock pulse, its J and K inputs are connected to Vcc or Vdd, where they will be “high” all the time. The next flip-flop need only “recognize” that the first flip-flop’s Q output is high to be made ready to toggle, so no AND gate is needed. However, the remaining flip-flops should be made ready to toggle only when all lower-order output bits are “high,” thus the need for AND gates.

Procedure

/* write all the steps invloved */

PROGRAM

/* Program for flipflops and verify its truth table in quartus using Verilog programming.

Developed by:YUVASREE S
RegisterNumber:25014102 */

RTL LOGIC UP COUNTER

TIMING DIAGRAM FOR IP COUNTER

TRUTH TABLE

RESULTS:
Thus the 4 Bit Synchronous Up Counter using verilog and validating their functionality is verified.
