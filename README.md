#### Introduction:
The project involves building a 4-bit ALU with 8 operations (2
arithmetic and 6 logical) and displaying the result on a seven-segment
display. Initially, it executes operations automatically by starting with a
selector value of 7, decrementing it, and showing each result until the
selector reaches zero. Then, it extends to include incrementing,
decrementing, and pausing functionalities controlled by a counter.
Finally, the circuit is enhanced to display operands, operation number, or
result based on a multiplexer, ensuring the seven-segment display shows
only non-blanking digits.


### Level 1:
8 ALU operation:
6 Logical: AND,OR,NAND,NOR , NOT A , NOT B
2 Arithmetic: Increment A , Increment B
We added four 8 x 1 muxes (IC 74251) with three bit select
wires to choose which operation we need and to see the output
each bit from one mux to see our final compiled result on seven
segments.


### Level 2 & 3:
3 JK flip flops and clock IC with some logic to create up down
counter. Our clock and increment decrement will be based on
control input. Giving user choice when to increment decrement
and when to stop.


### Level 4:
Two muxes (4 x2) to choose whether they wanna see
inputs , selectors or the answer.
Then we implemented another mux (8 x 4) to choose
whether the output is 0-9 or 10-15.
Also another logic to show only non-blanking output ie
when 01 is shown the output will only show 1.

### Conclusion:
In conclusion, the project successfully demonstrates the
construction and functionality of a 4-bit ALU with 8
operations, integrating both arithmetic and logical
functions. The design effectively displays results on a
seven-segment display, automating operation execution
with a decrementing selector. Enhanced features such as
incrementing, decrementing, and pausing operations add
flexibility and control, while the use of a multiplexer
ensures efficient display of operands, operation numbers,
or results, showing only non-blanking digits for clarity.
