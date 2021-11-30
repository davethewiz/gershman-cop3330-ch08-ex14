# Chapter 8, Exercise 14 - Using A Const Parameter in a Function

*NOTE: All function references in this readme are referring to the ```main.cpp``` file*

### Can we declare a non-reference function argument const (e.g., void f(const int);)?
Yes! This is shown in the function ```add2_const(const int num)``` function where one can easily use a const argument.

### What might that mean? Why might we want to do that?
Well, considering that ```const``` simply means that the variable is readonly and cannot be changed once intialized it can be used as a way of protecting the parameter
and making sure that it doesn't get modified while inside the function scope. 

For example, if we take the function ```modifyNum(int num)``` and instead make it so that the num is a ```const``` parameter. The function will throw an error because we modifying
a ```const``` variable marked as readonly.

However, it is important to keep in mind that the non-reference function argument will not be changed outside of the function.

### Why don’t people do that often?
Possibly because it may not be very useful as the argument will not be changing outside of the function and thus is already const by default outside of the function itself.
However, it has its uses from a readability standpoint if one uses const variables extensively and wants to remain consistent in their code.
