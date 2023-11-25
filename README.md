# Exp-03-Implementation-of-Half-Adder-and-Full-Adder-circuit
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
Developed by: Dharunyadevi.S
RegisterNumber: 23013594
```
module EX03DEHA(A,B,sum,carry);
input A,B;
output sum,carry;
xor(sum,A,B);
and(carry,A,B);
endmodule

module EX03DEFA(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
assign sum=((a^b)^c);
assign carry=((a&b)|(b&c)|(c&a));
endmodule
```
*/
Logic symbol & Truthtable
RTL realization
### RTL:
![image](https://github.com/DHARUNYADEVI/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147473847/44c661eb-0934-40ca-9962-b185ff55b082)
![image](https://github.com/DHARUNYADEVI/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147473847/b77f5364-54d9-4695-9370-394c760f97c5)
### TIMING DIAGRAM
![image](https://github.com/DHARUNYADEVI/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147473847/3a5b08f2-9788-484c-8974-0cec5fb6c992)
![image](https://github.com/DHARUNYADEVI/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147473847/f62f9a39-4dac-4863-8bae-bf4c40c6b147)
### TRUTH TABLE:
![image](https://github.com/DHARUNYADEVI/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/147473847/2ee5927e-fbbc-4303-8894-16c708044b2c)
### Result:
Thus the implementation of half adder and full adder verified successfully.
### TRUTH TABLE 

### Result:
