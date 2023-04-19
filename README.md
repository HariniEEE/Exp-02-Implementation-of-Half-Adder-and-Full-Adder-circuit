# Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
### AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

### Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

### Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

#### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

#### Figure -02 FULL ADDER 

### Procedure

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.
### 
Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

HALF ADDER

module Halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor (sum,a,b);
and (carry,a,b);
endmodule

FUL ADDER

module Fulladder (a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum = ((a^b)^c);
assign carry = ((a&b)|(b&c)|(c&a));
endmodule

Developed by: HARINI.E
RegisterNumber:  212222050017
*/
Logic symbol

![Logic symbol](https://user-images.githubusercontent.com/128949246/233090667-dbec0223-e267-463a-8ad9-6db20099aff9.jpeg)

RTL realization

### Output

Half Adder
![RTL half](https://user-images.githubusercontent.com/128949246/233091041-fac60f39-f3ea-4fa6-b236-9b32473d5a4d.jpeg)

Full Adder
![RTL full](https://user-images.githubusercontent.com/128949246/233091154-eb19cff4-fdc5-4091-9eed-9cc848f838e9.jpeg)


### TIMING DIAGRAM

Half Adder

![Timing half](https://user-images.githubusercontent.com/128949246/233091355-f42ed5aa-9336-4c80-a700-1077b8f255c4.jpeg)

Full Adder

![Timing full](https://user-images.githubusercontent.com/128949246/233091500-402225ad-bc08-4527-8609-ec274fc97083.jpeg)

### TRUTH TABLE 

HALF ADDER

![Truth half](https://user-images.githubusercontent.com/128949246/233091701-0c2327f7-633d-48de-9ae5-93891a3a0eb5.jpeg)

FULL ADDER

![Truth full](https://user-images.githubusercontent.com/128949246/233091790-1017446c-6bcc-40c1-8320-ed8c2bde2ce2.jpeg)


### Result:
Thus the implementation of Halfadder Fulladder Circuit are studied and the truthtable for different logic gates are verified.
