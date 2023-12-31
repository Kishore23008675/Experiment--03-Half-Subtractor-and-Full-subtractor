# Exp-04 Implementation of Half subtractor and Full subtractor circuit
## AIM:Exp-04 Implementation of Half subtractor and Full subtractor circuit
Name:KISHORE.A
Reference number:23008675


AIM:
To design a half subtractor and full subtractor circuit and verify its truth table in Quartus using Verilog programming.

Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime

Theory:

Subtractor circuits take two binary numbers as input and subtract one binary number input from the other binary number input. Similar to adders, it gives out two outputs, difference and borrow (carry-in the case of Adder). There are two types of subtractors.

Half Subtractor Full Subtractor:
Half Subtractor:
The half-subtractor is a combinational circuit which is used to perform subtraction of two bits. It has two inputs, X (minuend) and Y (subtrahend) and two outputs D (difference) and B (borrow). To perform x - y, we have to check the relative magnitudes of x and y. If x ;;, y, we have three possibilities: 0 - 0 = 0, 1 - 0 = 1, and 1 - I = 0. The result is called the difference bit. If x < y, we have 0 - I, and it is necessary to borrow a 1 from the next higher stage. The I borrowed from the next higher stage adds 2 to the minuend bit, just as in the decimal system a borrow adds 10 to a minuend digit. With the minuend equal to 2, the difference becomes 2 - I = 1. The half-subtractor needs two outputs. One output generates the difference and will be designated by the symbol D. The second output, designated B for borrow, generates the binary signal that informs the next stage that a I has been borrowed. 

![Screenshot 2023-12-29 232821](https://github.com/Kishore23008675/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/144979375/c2eb32ed-9afb-45e7-831a-9057b4c3c4c5)


Sum = X'Y+XY' = X ⊕ Y Carry=X'Y

Full Subtractor:
A full subtractor is a combinational circuit that performs subtraction involving three bits, namely minuend, subtrahend, and borrow-in . It accepts three inputs: minuend, subtrahend and a borrow bit and it produces two outputs: difference and borrow. full-subtractor6

Diff = A ⊕ B ⊕ Bin B = A'Bin + A'B + BBin

Procedure:

1.Use module projname(input,output) to start the Verilog programmming.

2.Assign inputs and outputs using the word input and output respectively.

3.Use defined keywords like wire,assign and required logic gates to represent the boolean expression.

4.Use each output to represnt onre for differnce and the other for borrow.

5.End the verilog program using keyword endmodule

Program:
Half Subtracter:
![Screenshot 2023-12-29 232521](https://github.com/Kishore23008675/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/144979375/ae006828-1da2-4b16-b6e7-1687e141026c)


Full Subtracter:
![Screenshot 2023-12-29 232514](https://github.com/Kishore23008675/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/144979375/423d296d-7713-466f-bfa0-b360c787a146)


Truthtable:
Half Subtracter:
![Screenshot 2023-12-29 232505](https://github.com/Kishore23008675/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/144979375/bc4c6daf-7a6c-4a15-91b3-2f7840b90adf)


Full Subtracter:
![Screenshot 2023-12-29 232456](https://github.com/Kishore23008675/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/144979375/3f5d09cb-c9d4-4cec-82fe-0ded7c2ed5c7)


RTL realization:
Half Subtracter:
![Screenshot 2023-12-29 232447](https://github.com/Kishore23008675/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/144979375/33309bb3-aca8-476c-b670-410177477b9a)


Full Subtracter:
![Screenshot 2023-12-29 232428](https://github.com/Kishore23008675/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/144979375/4ee10f6f-d85e-42b3-b72b-375c9e045817)


Output:
Half Subtracter:

![Screenshot 2023-12-29 232347](https://github.com/Kishore23008675/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/144979375/6bb97f59-973c-45c0-a737-de99b53c024f)


Full Subtracter:
![Screenshot 2023-12-29 232143](https://github.com/Kishore23008675/Experiment--03-Half-Subtractor-and-Full-subtractor/assets/144979375/e92ab373-c794-4fc9-8a89-a99d0ea50161)


Result:
Thus the half subtractor and full subtractor circuits are designed and the truth tables is verified using quartus software.
