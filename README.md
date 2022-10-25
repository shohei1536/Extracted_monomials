# Extracted_monomials
_Appendix for the paper "Linearizing Robotic Manipulator's Dynamics Using Koopman Operator and Applying Generalized Predictive Control"_

These are the monomials that appear in the expansion of the dynamics equation for the robot arm, and which were used to linearize using the Koopman operator.

**Contents of the files**

The top row of the Excel file is the simplest base monomials that makes up the monomials that are important for describing robot dynamics. Each subsequent row represents the desired monomials, expressed as a multiplication of the base monomials. The number in each row represents the order of power of the base monomial.

**Exsample**

If robot's dynamics is described using Koopman operator matrix (K) and observables vector (x) as follow:

$$x_{t+1} = K x_{t}$$

And 

$$x = [ q1,  q1sin(q1),  q2^{2}sin(q2),  q1q2sin(q1) ]^{T}$$

Then the x is expressed in the Excel file as follows

| Base monomials | q1  | q2  | sin(q1) | sin(q2) | 
| -------------- | --- | --- | ------- | -------------- | 
| monomial #1    | 1   | 0   | 0       | 0              | 
| monomial #2    | 1   | 0   | 1       | 0              | 
| monomial #3    | 0   | 2   | 0       | 1              | 
| monomial #4    | 1   | 1   | 1       | 0              | 
