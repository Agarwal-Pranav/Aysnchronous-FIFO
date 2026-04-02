# Asynchronous System Design

## Overview
This project focuses on the design and implementation of an asynchronous system where operations are performed without a global clock signal. Instead of relying on a clock, the system uses handshaking protocols and event-driven communication to transfer data. This approach improves power efficiency and eliminates clock-related issues such as skew and jitter.

## Objectives
- Design a clock-independent digital system  
- Implement handshake-based communication  
- Reduce power consumption  
- Improve robustness against timing variations  
- Explore delay-insensitive design techniques  

## Key Concepts
- Asynchronous Circuits  
- Handshaking Protocol (Request/Acknowledge)  
- Muller C-Element  
- Hazard-Free Design  
- Delay Insensitivity  
- Event-Driven Operation  

## Architecture
The system consists of the following components:

- Input Stage: Accepts input data and generates request signals  
- Control Logic: Manages synchronization using handshake signals  
- Processing Block: Performs the required computation  
- Output Stage: Sends output data along with acknowledgment  

## Handshake Protocol
A 4-phase handshake protocol is used:

1. Sender asserts Request (Req)  
2. Receiver processes data and asserts Acknowledge (Ack)  
3. Sender deasserts Request (Req)  
4. Receiver deasserts Acknowledge (Ack)  

## Implementation Details
- Hardware Description Language: Verilog / VHDL  
- Simulation Tools: ModelSim / Cadence / Vivado  
- Design Approach: Event-driven and delay-insensitive logic  


## How to Run
1. Clone the repository  
2. Open the project in a simulation tool  
3. Compile all source files  
4. Run the testbench  
5. Observe waveform outputs  

## Results
- Correct handshake operation verified  
- No dependency on clock signal  
- Reduced switching activity  
- Reliable performance under varying delays  

## Challenges
- Handling hazards and race conditions  
- Complex timing verification  
- Limited tool support compared to synchronous systems  

## Future Work
- Design asynchronous pipelines  
- Implement GALS systems  
- Optimize power and area  
- FPGA-based implementation  

## References
- Asynchronous Circuit Design literature  
- IEEE research papers on asynchronous systems  
- Digital VLSI design textbooks  
