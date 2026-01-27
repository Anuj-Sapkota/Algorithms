# How to write an Algorithm

            Algorithm Swap(a,b)
            {
                temp = a 
                a = b
                b = temp
            }


## How to Analyze an Algorithm
### 1. Time
        How much time is it taking
        Must be time efficient.
### 2. Space
        How much memory does it consume
### 3. Network or Data consumption
        How much data is transfered
        Can it be reduced or compressed?
### 4. Power consumption

### 5. CPU Registers does it consume



---
---
# Analyzation

## 1. Time Analysis

            Algorithm Swap(a,b)
            {
                temp = a -----> 1 unit
                a = b --------> 1 unit
                b = temp -----> 1 unit
            }

### 1. Every symbol statement takes one unit of time
####  1.1. Simple statements not the nested ones 
   
### 2. If an algorithm is calling another algorithm then, we would need to analyze the other algorithm's time function as well
   
    From the above function we see that we get 3 units of time function meaning:
        f(n) = 3 
    
    But, if there was a statement like:
        x = 5*6 + 7*8
    If we are calculating basic time function we say this as one units. 
    But, in reaity as this code gets converted into machine level code, it takes 3 steps/units.
    If the task requires us to go into very detail then we should do deep analysis, if not then basic aalysis is also fine.

## 2. Space Analysis

    From the same example we also calculate space as one unit per statement, making the above algorithm, 3 units of space function.
        s(n) = 3

As both of them are constant we represent them as the order of 1 or

    O(1)