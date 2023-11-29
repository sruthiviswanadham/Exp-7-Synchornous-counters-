# Exp-6-Synchornous-counters - up counter and down counter 
### AIM: To implement 4 bit up and down counters and validate  functionality.
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

## UP COUNTER 
The counter is a digital sequential circuit and here it is a 4 bit counter, which simply means it can count from 0 to 15 and vice versa based upon the direction of counting (up/down). 

The counter (“count“) value will be evaluated at every positive (rising) edge of the clock (“clk“) cycle.
The Counter will be set to Zero when “reset” input is at logic high.
The counter will be loaded with “data” input when the “load” signal is at logic high. Otherwise, it will count up or down.
The counter will count up when the “up_down” signal is logic high, otherwise count down

Since we know that binary count sequences follow a pattern of octave (factor of 2) frequency division, and that J-K flip-flop multivibrators set up for the “toggle” mode are capable of performing this type of frequency division, we can envision a circuit made up of several J-K flip-flops, cascaded to produce four bits of output.
The main problem facing us is to determine how to connect these flip-flops together so that they toggle at the right times to produce the proper binary sequence.
Examine the following binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1:
Binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1.

Note that each bit in this four-bit sequence toggles when the bit before it (the bit having a lesser significance, or place-weight), toggles in a particular direction: from 1 to 0.



 
 

Starting with four J-K flip-flops connected in such a way to always be in the “toggle” mode, we need to determine how to connect the clock inputs in such a way so that each succeeding bit toggles when the bit before it transitions from 1 to 0.

The Q outputs of each flip-flop will serve as the respective binary bits of the final, four-bit count:

 
 

Four-bit “Up” Counter
![image](https://user-images.githubusercontent.com/36288975/169644758-b2f4339d-9532-40c5-af40-8f4f8c942e2c.png)



## DOWN COUNTER 

As well as counting “up” from zero and increasing or incrementing to some preset value, it is sometimes necessary to count “down” from a predetermined value to zero allowing us to produce an output that activates when the zero count or some other pre-set value is reached.

This type of counter is normally referred to as a Down Counter, (CTD). In a binary or BCD down counter, the count decreases by one for each external clock pulse from some preset value. Special dual purpose IC’s such as the TTL 74LS193 or CMOS CD4510 are 4-bit binary Up or Down counters which have an additional input pin to select either the up or down count mode.
![image](https://user-images.githubusercontent.com/36288975/169644844-1a14e123-7228-4ed8-81a9-eb937dff4ac8.png)


4-bit Count Down Counter
### Procedure
Create a new project in Quartus2 software .
Name the project as uc for upcounter and dc for down counter.
Create a new verilog hdl file in the project file.
Name the module declare as dc and uc for down counter and upcounter.
Within the module declare input and output variables.
Create a loop using if-else with condition parameter as reset.
End the loop.
End the module



### PROGRAM 
/*
Program for flipflops  and verify its truth table in quartus using Verilog programming.

Developed by:V.Sai Sruthi 
RegisterNumber: 23012602 

## Up Counter

## Code

![image](https://github.com/sruthiviswanadham/Exp-7-Synchornous-counters-/assets/151760421/88cfd8b8-d680-4f73-8629-6833261e0418)

## RTL Diagram

![image](https://github.com/sruthiviswanadham/Exp-7-Synchornous-counters-/assets/151760421/1ca8005b-ae68-4dd8-a9af-739438396c27)

## Timing Diagram

![image](https://github.com/sruthiviswanadham/Exp-7-Synchornous-counters-/assets/151760421/cdf2f7ec-aeff-46e3-a3a2-ce2ebd4573d1)

## Truth Table

![image](https://github.com/sruthiviswanadham/Exp-7-Synchornous-counters-/assets/151760421/a9ccee61-2c49-49b0-af37-95089b2f39ff)

## Down Counter

## Code

![image](https://github.com/sruthiviswanadham/Exp-7-Synchornous-counters-/assets/151760421/5b039410-f616-4a2a-9a9d-5490b3e6c7be)

## RTL Diagram

![image](https://github.com/sruthiviswanadham/Exp-7-Synchornous-counters-/assets/151760421/cb6a0486-6ee5-49c0-8a4a-0378fcadf550)

## Timing Diagram

![image](https://github.com/sruthiviswanadham/Exp-7-Synchornous-counters-/assets/151760421/018c51dd-61ed-4c45-b5f0-341b2bedea12)

## Truth Table

![image](https://github.com/sruthiviswanadham/Exp-7-Synchornous-counters-/assets/151760421/3363c32f-cb46-4831-af00-a05e983481c6)

## Results

 Thus synchornous counters up counter and down counter circuit are studied and the truth table for different logic gates are verified.






