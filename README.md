# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit

# Implementation-of-Half-Adder-and-Full-Adder-circuit
## AIM :
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

## Equipments Required :
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

## Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

## Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d25.png)

### Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

### Figure -02 FULL ADDER 

## Procedure :

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.

## Program :

Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

Developed by: MOHAMED ATHIL B

RegisterNumber: 212222230081

### Half Adder 
```
module HalfAdder(A,B,sum,carry);
input A,B;
output sum,carry;
assign sum= A^B;
assign carry = A&B;
endmodule
```

### Full Adder 
```
module FullAdder(A,B,Cin,sum,carry);
input A,B,Cin;
output sum,carry;
assign sum= A^B^Cin;
assign carry = (A&B)|((A^B)&Cin);
endmodule
```

## RTL DIAGRAM :

### Half Adder
![image](https://github.com/Bmohamedathil/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119560261/71b90843-2114-4f45-bf35-3fd71f93d922)

### Full Adder
![image](https://github.com/Bmohamedathil/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119560261/960e894c-2256-4df8-8aff-ec514cce87ac)

## Truth Table :

### Half Adder
![image](https://github.com/Bmohamedathil/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119560261/d7bd0794-3f1e-422f-afc3-07c4a6350be6)

### Full Adder
![image](https://github.com/Bmohamedathil/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119560261/7e5b279c-83be-4c9c-a990-084528939154)

## Output Waveform :

### Half Adder
![image](https://github.com/Bmohamedathil/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119560261/c1ff2d8c-5819-46b8-aa0e-b92888042727)

### Full Adder
![image](https://github.com/Bmohamedathil/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/119560261/bdbe5ee6-b913-4e58-b905-0dac213922c9)

### Result :
Thus, a Half Adder and Full Adder Circuit is Designed to Verify its Truth Table in Quartus Using Verilog Programming.
