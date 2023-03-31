# ALU Project

On this project i’m using Logisim, to make the circuits and all visual parts of ALU.

The developed ALU is an integrated circuit that should receive two 4-bit numbers (a and b), one for the sign and three for the magnitude, and perform the requested operations, displaying the result on a 7-segment display.

For this, the integrated circuit must have the following functions:

Receive the 4-bit numbers a and b, with one bit for the sign and three for the magnitude;
Perform addition, subtraction, 2's complement, equality, greater than, less than, AND and XOR operations according to the user's selections S();
Store the result in an output register;
Convert the result to a format compatible with the 7-segment display, displaying the result in decimal or hexadecimal form.
Each selection S() should correspond to a specific operation, as follows:

| S2 | S1 | S0 |  |
| --- | --- | --- | --- |
| 0 | 0 | 0 | F= a+b |
| 0 | 0 | 1 | F= a-b |
| 0 | 1 | 0 | 2's compl. of b (F=~b+1) |
| 0 | 1 | 1 | F=(a=b)? |
| 1 | 0 | 0 | F=(a>b)? |
| 1 | 0 | 1 | F=(a<b)? |
| 1 | 1 | 0 | bitwise AND (F=(a AND b)) |
| 1 | 1 | 1 | bitwise XOR (F=(a XOR b)) |

Thus, by selecting one of the options, the ALU must perform the corresponding operation and display the result on the 7-segment display.