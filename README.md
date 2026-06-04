# SIMULATION-OF-MEAN-AND-VARIANCE-USING-SCILAB-
__AIM:__

To write a program for mean, variance and cross correlation in SCILAB and verify the output. 

__EQUIPMENTS NEEDED:__

.Computer with i3 Processor 

.SCI LAB 

__ALGORITHM:__

1. Define the Function: Specify the function you want to simulate. For example, 
f(x)=sin⁡(x)f(x)=sin(x) or any other function. 
2. Generate Sample Points: Decide on the range and the number of sample points. Generate 
these sample points within the desired range. 
3. Evaluate the Function: Compute the function values at each of these sample points. 
4. Compute Mean, Variance and Cross Correlation: Use Scilab's functions to calculate the 
mean and variance of the computed function values. 
5. Display Results: Output the computed mean variance and Cross Correlation 

__PROCEDURE:__ 

1.Refer Algorithms and write code for the experiment. 

2.Open SCILAB in System 

3.Type your code in New Editor 

4.Save the file 

5.Execute the code If any Error, correct it in code and execute again 
  
6.Verify the generated results

__PROGRAM__:
### Mean
```
clear; 
clc;
clear;

function X=f(x),
z=3*(1-2*x)^2,
X=x*z
endfunction
a=0;
b=1;
EX=intg(a,b,f);
function Y=c(y)
z=3*(1-2*y)^2,
Y=y*z
endfunction
EY=intg(a,b,c);
disp(EX,"i)Mean of X =")
disp(EY," Mean of Y =")
```
### Variance
```
function X=g(x),
z=3*(1-2*x)^2
X=x^2*z
endfunction 
a=0;
b=1;
EX2=intg(a,b,g);
function Y=h(y)
z=3*(1-2*y)^2,
Y=y^2*z
endfunction
EY2=intg(a,b,h);
vX2=EX2-(EX)^2;
vY2=EY2-(EY)^2;
disp(vX2,"ii)Variance of X");
disp(vY2," Variance of Y");
```
### Cross Correlation
```
x= input("type in the reference sequence=");
y= input("type in the second sequence=");
n1=max(size(y))-1;
n2=max(size(x))-1;
r=corr(x,y,n1);
plot2d3('gnn',r);

```
### Tabulation
<img width="489" height="845" alt="image" src="https://github.com/user-attachments/assets/ab26e079-85e3-4564-8320-de9360d321f0" />

__OUTPUT GRAPH:__
<img width="1481" height="672" alt="Screenshot 2026-05-29 103046" src="https://github.com/user-attachments/assets/7daf8b3e-c53d-45c6-bc1b-ba89593542b3" />



__RESULT:__
Thus mean, variance and cross correlation are executed in Scilab and outputs are verified.

