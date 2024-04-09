# Rolling Average Calculation for 16-bit Numbers in VHDL

## Introduction

This project focuses on implementing a rolling average calculation for 16-bit numbers using [VHDL](https://en.wikipedia.org/wiki/VHDL) and an [FPGA board (Basys3)](https://digilent.com/reference/programmable-logic/basys-3/start). The rolling average is calculated over a window of 2, 4, 8, or 16 numbers. It demonstrates a deep understanding of basic hardware components such as registers, frequency dividers, pseudo-random number generators, full-adders, and more. Additionally, it provides an excellent opportunity to improve debugging skills, crucial in digital system design.

## Design Overview

The project utilizes various hardware components to achieve the rolling average calculation:

1. **Registers**: Used for storing input numbers and intermediate results.
2. **Frequency Dividers**: To control the clock frequency and synchronize signals.
3. **Pseudo-random Number Generators**: Generating random numbers for testing.
4. **Full-Adders**: Adding 16-bit numbers.
5. **Multiplexers**: Selecting the number of samples for the rolling average.
6. **Controllers**: Coordinating the operation of different components.

## Implementation Steps

1. **Design Specification**: Define the requirements, including the window size and input/output specifications.
2. **VHDL Implementation**: Write VHDL code for each component based on the design specification.
3. **Simulation**: Verify the correctness of the VHDL code using simulation tools like ModelSim.
4. **FPGA Implementation**: Synthesize the VHDL code and program the FPGA board.
5. **Testing and Debugging**: Test the functionality of the implemented design on the FPGA board, identify and fix any issues.
6. **Performance Optimization**: Optimize the design for speed and resource utilization if required.
7. **Documentation**: Document the design, implementation details, test results, and any challenges faced during the project.

## Example Rolling Average Calculation

Suppose we want to calculate the rolling average of 4 numbers: \( A_1, A_2, A_3, \) and \( A_4 \). The rolling average at each step is calculated as:

\[ \text{Rolling Average} = \frac{{A_1 + A_2 + A_3 + A_4}}{4} \]

As a new number arrives, the oldest number is replaced, and the rolling average is updated accordingly.

## Conclusion

The rolling average calculation project for 16-bit numbers in VHDL provides a hands-on experience in digital system design, encompassing various hardware components and requiring meticulous debugging skills. Through this project, one gains a deeper understanding of FPGA-based digital systems and strengthens problem-solving abilities in hardware design.

![Basys3 FPGA Board](https://github.com/bartha26/Rolling-Average/blob/main/res/Screenshot%202024-04-09%20190226.png)
*Figure 1: Basys3 FPGA Board*

![VHDL Code Example](file:///C:/Users/TudorB/Pictures/Screenshots/Screenshot%202024-04-09%20190743.png)
*Figure 2: Example VHDL Code*

![VHDL Code Example 1](file:///C:/Users/TudorB/Pictures/Screenshots/Screenshot%202024-04-09%20191029.png)
*Figure 3: Example VHDL Code Register*

By combining theoretical knowledge with practical implementation, this project offers a comprehensive learning experience in digital system design and FPGA programming.

## References

Provide references to textbooks, online resources, or tutorials that were helpful during the project.

1. Smith, John. "Digital System Design Fundamentals." Publisher, Year.
2. "Basys3 FPGA Board User Guide." Available online at: [link](https://www.digilentinc.com/)
3. "VHDL Tutorial." Available online at: [link](https://www.vhdltutorial.com/)
