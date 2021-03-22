# EE SEM 1 PROJECT

The aim of the project is to construct the digital circuit of a 5 bit full adder using logic gates.

Here is a brief idea about Binary adders. Mainly there are two types of Adder: Half Adder and Full Adder. In half adder we can add 2-bit binary numbers but we cant add carry bit in half adder along with the two binary numbers. But in Full Adder Circuit we can add carry in bit along with the two binary numbers. We can also add multiple bits binary numbers by cascading the full adder circuits.

# Full Adder Circuit:
<img src="https://github.com/Anshnrag02/Five-Bit-Adder/blob/main/images/Full-Adder-Circuit%20(1).png?raw=true">
So we know that Half-adder circuit has a major drawback that we do not have the scope to provide ‘Carry in’ bit for addition. In case full adder construction, we can actually make a carry in input in the circuitry and could add it with other two inputs A and B. So, in the case of Full Adder Circuit we have three inputs A, B and Carry In and we will get final output SUM and Carry out. So, A + B + CARRY IN = SUM and CARRY OUT.

As per mathematics, if we add two half numbers we would get full number, same thing is happening here in full adder circuit construction. We add two half adder circuits with an extra addition of OR gate and get a complete full adder circuit.

# Construction
Full adder circuit construction is shown in the above block diagram, where two half adder circuits added together with a OR gate. The first half adder circuit is on the left side, we give two single bit binary inputs A and B. It will produce two outputs, SUM and Carry out. First half adder circuit’s SUM output is further provided to the second half adder circuit’s input. We provided the carry in bit across the other input of second half order circuit. Again it will provide SUM out and Carry out bit. This SUM output is the final output of the Full adder circuit. On the other hand the Carry out of First half adder circuit and the Carry out of second adder circuit is further provided into OR logic gate. After logic OR of two Carry output, we get the final carry out of full adder circuit.
The Final Carry out represents the most significant bit or MSB. 
If we see the actual circuit inside the full adder, we will see two Half adders using XOR gate and AND gate with an additional OR gate.

# Truth Table 

We can also express the full adder circuit construction in Boolean expression.<br>

<img src="https://github.com/Anshnrag02/Five-Bit-Adder/blob/main/OIP%20(4).jfif">

For the case of SUM, We first XOR the A and B input then we again XOR the output with Carry in. So, the Sum is (A XOR B) XOR C.
We can also express it with (A ⊕ B) ⊕ Carry in.
Now, for the Carry out, it is A AND B OR Carry in (A XOR B), which is further represented by A.B + (A ⊕ B).

# Cascading Full Adders

As of now, we described the construction of single bit adder circuit with logic gates. But what if we want to add two more than one bit numbers?<br>
<img src="https://github.com/Anshnrag02/Five-Bit-Adder/blob/main/images/Cascading-Adder-Circuits.png?raw=true">
Here is the advantage of full adder circuit. We can cascade single bit full adder circuits and could add two multiple bit binary numbers. This type of cascaded full adder circuit is called as Ripple Carry Adder circuit.

In case of Ripple Carry Adder circuit, Carry out of the each full adder is the Carry in of the next most significant adder circuit. As the Carry bit is ripple into the next stage, it is called as Ripple Carry Adder circuit. Carry bit is rippled from the left to right (LSB to MSB).

# Demonstration
<img src="https://github.com/Anshnrag02/Five-Bit-Adder/blob/main/images/Full-Adder-Circuit-using-74LS283N-in-action.jpg?raw=true">

We will use a full adder logic chip and add 4 bit binary numbers using it. We will use TTL 4 bit binary adder circuit using IC 74LS283N.
