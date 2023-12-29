## NAME : GOKUL SACHIN K
## REGISTER NUMBER:23004843
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
1.Use module projname(input,output) to start the Verilog programmming.
2.Assign inputs and outputs using the word input and output respectively.
3.Use defined keywords like wire,assign and required logic gates to represent the boolean expression.
4.Use each output to represnt onre for differnce and the other for borrow. 5.End the verilog program using keyword endmodule
### PROGRAM 
## HALF ADDER
```
module halfadder(a,b,sum,carry);
input a,b;
output sum,carry;
xor(sum,a,b);
and(carry,a,b)
endmodule
```
## FULL ADDER
```
module halfadder(a,b,c,sum,carry);
input a,b,c;
output sum,carry;
xor(sum,a,b,c);
assign carry=a&b | b&c | a&c
endmodule
```
### RTL
## HALF ADDER:
![HALF ADDER](https://github.com/vksachin2018/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149366019/5768fbe5-b14a-40b2-bd03-f25f247d790c)


## FULL ADDER
![FULL ADDER](https://github.com/vksachin2018/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149366019/c580d398-2152-490e-a413-ded5334d00eb)

### TRUTH TABLE 
## HALF ADDER:
![HALF ADDER TT](https://github.com/vksachin2018/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149366019/083501f6-0442-4bbe-b35e-7fed42533389)

## FULL ADDER:
![FULL ADDER TT](https://github.com/vksachin2018/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149366019/55674f58-32a3-4dad-982f-a5d313a3fa7f)

## OUTPUT:
## HALF ADDER:

![HALF ADDER OUTPUT](https://github.com/vksachin2018/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149366019/047a73b6-dfdd-44e7-8af0-25e6e3e82651)

## FULL ADDER:
![FULL ADDER OUTPUT](https://github.com/vksachin2018/Exp-02-Implementation-of-Half-Adder-and-Full-Adder-circuit/assets/149366019/fbd42dfb-acef-4729-93df-160689e26610)

### Result:
