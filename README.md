AIM:
To design a half adder and full adder circuit and verify its truth table in Quartus using Verilog programming.

Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
Adders are digital circuits that carry out addition of numbers.

 Half Adder
Half adder is a combinational circuit that performs simple addition of two binary numbers. The input variables designate the augend and addend bits; the output variables produce the sum and carry. It is necessary to specify two output variables because the result may consist of two binary digits.

Sum = A’B+AB’ =A ⊕ B Carry = AB

 Full Adder
Full adder is a digital circuit used to calculate the sum of three binary bits. It consists of three inputs and two outputs. Two of the input variables, denoted by A and B, represent the two significant bits to be added. The third input, Cin, represents the carry from the previous lower significant position. Two outputs are necessary because the arithmetic sum of three binary digits ranges in value from 0 to 3, and binary 2 or 3 needs two digits. The two outputs are sum and carry.

Sum =A’B’Cin + A’BCin’ + ABCin + AB’Cin’ = A ⊕ B ⊕ Cin Carry = AB + ACin + BCin

 ![image](https://user-images.githubusercontent.com/36288975/163552156-a13e5a56-c638-4110-97d9-8896907c8d Figure -01 HALF ADDER 


![image](https://user-images.githubusercontent.com/36288975/163552057-b3547877-6d07-45b4-b7e0-bcfebfad9e1d.png)

 Figure -02 FULL ADDER 

Procedure 

Connect the supply (+5V) to the circuit
Switch ON the main switch
If the output is 1, then the led glows.

DEVELOPED BY :K.ABINAYA
REGISTER NUMBER : 22005179

Program:
/*
Program to design a half adder and full adder circuit and verify its truth table in quartus using Verilog programming.

HALF ADDER  

module HalfAdder(a,b,sum,carry

input a,b;

output sum,carry;

xor(sum,a,b);

and(carry,a,b);

endmodule  

FULL ADDER  

module FullAdder(a,b,c,sum,carry);

input a,b,c;

output sum,carry;

assign sum = ((a^b)^c);

assign carry = ((a&b)|(b&c)|(c&a));

endmodule  


LOGIC GATES

![Screenshot (18)](https://user-images.githubusercontent.com/121557762/211152628-66ca305c-21d7-4c5c-a20e-0a2c13857464.png)


RTL
OUTPUT

HALF ADDER


![Screenshot (19)](https://user-images.githubusercontent.com/121557762/211152630-2d538111-139d-4d96-a6ca-c13f7d1a47b0.png)

FULL ADDER 

![Screenshot (20)](https://user-images.githubusercontent.com/121557762/211152638-15577c3a-d503-4231-8571-fb07a33c01a6.png)

TIMING DIAGRAM 

HALF ADDER 

![Screenshot (21)](https://user-images.githubusercontent.com/121557762/211152651-60153ae2-0078-425d-89f4-d4e8b459c614.png)


FULL ADDER 

![Screenshot (22)](https://user-images.githubusercontent.com/121557762/211155606-dc611ac0-6f55-4d2e-aef2-2e991f1ba8da.png)



TRUTH TABLE 

HALF ADDER 

![Screenshot (23)](https://user-images.githubusercontent.com/121557762/211152662-0d0441f8-d3a8-4a40-9560-f00ea4a1a1d2.png)

FULL ADDER

![Screenshot (24)](https://user-images.githubusercontent.com/121557762/211152673-4dd42144-6dd1-42c9-a2a5-5daa27a4b9fb.png)



Result:Thus the implementation of half adder and full adder circuit are stuided and the truth table for different logic gates are verified
