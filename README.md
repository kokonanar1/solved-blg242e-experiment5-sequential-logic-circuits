Download Link: https://assignmentchef.com/product/solved-blg242e-experiment5-sequential-logic-circuits
<br>
In this experiment, you will implement sequential logic circuits by using the Verilog. Refreshing your knowledge on followings is useful to implement this experiment;

<ul>

 <li>How to analyze a given sequential circuits,</li>

 <li>How to design circuits with Mealy and Moore models,</li>

</ul>

You can utilize 7th and 8th slides of BLG231E-Digital Circuits course for this experiment. Also, you can use the modules that you have implemented in previous experiments.

<h1>2      Preliminary</h1>

Please complete the preliminary work and explain their in detail in your report.

<ul>

 <li>Analyze the circuit in Part-1 to create a state transition table and a state chart.</li>

 <li>Design and draw the circuit to implement in Part-2 with the minimum number of logic gates.</li>

</ul>

<h1>3      Experiment</h1>

Part 1

In this part, you have to implement the circuits in Figure 1 by using Verilog. You need to use <strong>different type flip flop modules</strong>, <strong>logic gates </strong>and <strong>clock signal </strong>to synchronize the circuit. Report the state transition table for this circuits and draw state diagram graphically. Also, show your simulation results (timing diagram) by testing your circuits.

You may add reset input to set initial values. <strong>NOTE: </strong>You cannot use always block.

1

<em>Experiment 5 Sequential Logic Circuits</em>

Figure 1: Sequential circuit with flip flops

Part 2

Build a 4 bit counter circuit that counts 0 to 14 in a circular way (in an other word, after 14, it returns to 0). Block diagram of the counter is given in Figure 2. Here, input X is the counting direction. X=0 means counting DOWN (2-1-0-14-13-12-…) while X=1 means counting UP (13-14-0-1-2…). You have to use D or JK flip flop modules instead of reg type in this part.

Figure 2: 4 bit counter block diagram.

Part 3

In this part, please implement a 16-bit up-down counter that have 16-bit input data, load, clock, direction, 3-bit increment/decrement value and clear inputs using <strong>reg </strong>type parameter and <strong>always block</strong>. The output of the module is 16-bit current value of the counter. When the clear input is zero, current value of the counter becomes zero. When the load input is zero, input data is loaded to the the current value register. Otherwise, the current value of the counter is increased or decreased according to direction input and increment/decrement value on each positive edge of the clock input. For example, when the direction input is one and increment/decrement value is 2 (and clear=1, load=1), the module increases the counter with number 2. When the direction input is zero and decrement number is 3, the module decreases the counter with 3.

2

Part 4

In this part, implement below counter modules using 16-bit up-down counter module that is implemented in Part 3;

<ul>

 <li>A counter that counts up from 0 to 40 in circular way with increment value 2.</li>

 <li>A counter that counts up from 350 to 371 in circular way with increment value 3</li>

 <li>A counter that counts down from 93 to 5 in circular way with decrement value 4.</li>

 <li>A counter that counts up from 22525 to 22535 in circular way with increment value</li>

</ul>

1.

Each module has clock input, initiate input, and 16-bit current value output. When the initiate input is zero, your counter will be set any number which is in the range of the counter. For example, for the 0 to 20 counter, you can set the current value as 0 when the initiate input is zero. The clock input will be used for update the current value.