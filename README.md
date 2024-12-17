# BOOLEAN_FUNCTION_MINIMIZATION

**AIM:**

To implement the given logic function verify its operation in Quartus using Verilog programming.

F1= A’B’C’D’+AC’D’+B’CD’+A’BCD+BC’D 

F2=xy’z+x’y’z+w’xy+wx’y+wxy 

**Equipment Required:**

Hardware – PCs, Cyclone II , USB flasher

**Software – Quartus prime**

**Theory**

**Logic Diagram**

**Procedure**

1.	Type the program in Quartus software.

2.	Compile and run the program.

3.	Generate the RTL schematic and save the logic diagram.

4.	Create nodes for inputs and outputs to generate the timing diagram.

5.	For different input combinations generate the timing diagram.


**Program:**

/* Program to implement the given logic function and to verify its operations in quartus using Verilog programming. 

Developed by:ROSHINI A  RegisterNumber:24002364
module exp22(A,B,C,D,F1);
input A,B,C,D;
output F1;
wire x1,x2,x3,x4,x5;
assign x1=(~A)&(~B)&(~C)&(~D);
assign x2=(A)&(~C)&(~D);
assign x3=(~B)&(C)&(~D);
assign x4=(~A)&(B)&(C)&(D);
assign x5=(B)&(~C)&(D);
assign F1=x1|x2|x3|x4|x5;
endmodule


**RTL realization**





![image](https://github.com/user-attachments/assets/a1083994-b94d-4043-a854-00f6d3e611ac)


**Truth table**




![313054208-ee2fd841-7a98-4ded-9637-76f31327d8b3](https://github.com/user-attachments/assets/5bd6ae88-7ee3-4a24-9e86-f9559cccd124)


**Waveform**





![313054423-bce7ad1d-dd00-451f-b1b0-8797ea332973](https://github.com/user-attachments/assets/94d330d2-ce42-4172-9f18-984c6d28693a)



**Result:**

Thus the given logic functions are implemented using and their operations are verified using Verilog programming.

