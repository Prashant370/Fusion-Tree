Team Members Name:

Prashant Kumar      2022csb1202<br>
Pranav Bhole        2022csb1103<br>
Kartikey Sahu       2022csb1087<br>

Instructor : Dr. Anil Shukla || Mentor : Soumya Sarkar  <br>

Project Name:- Implementation of Fusion Tree in C++ <br>

![image](https://github.com/pranavbhole123/CS201project/assets/120297405/003ab476-448e-45e9-a4bb-5c836d980ab6)


General instruction
------------------------

How to compile and run the code  <br>

(1) check that package is install in linux or other device <br>
(2) gcc file_name.c for compile  <br>
(3) ./a.out for run the code  <br>

---------------------------------------------------------------

---------------------------------------------------------------
When we compile and run the code in ```fusiontree.cpp``` 
we should obtain the following output:

```
Application of Fusion Tree
(1) Fusion Tree size: 5
(2) After Sorting : 1 4 9 16 25 
(3) Queried elements:
predecessor of 3: 1
predecessor of 16: 16
predecessor of 0: -1
successor of 0: 1
successor of 10: 16
```

## Summary ## <br>

A Fusion Trees is a static Data Structure that allows for predecessor queries in constant
time on a set of constant size of numbers, but that requires significant large word sizes
to be implemented in a computer that  follows  the standard word ram model. In this work,
we provide the C++ code and reference to our implementation of fusion trees that performs
predecessor queries with a constant number of calls .Our Fusion Tree is restriced to word
size so we are implementing only for w=32 . as we are implementing in c++ if one can
implement in python or similar programming language it can go upto a certain significant
size but beyond that its depend on machine .

Challenges <br>

(1) Large Integer Sizes <br>

Implementing data structures like Fusion Trees in languages with large integer sizes
(e.g., python) is generally straightforward, but it can become challenging when
dealing with languages that have limited support for very large integers like C++. Working 
with integers of size 10^18 or greater may not be feasible in some languages, and 
handling such large values efficiently becomes a challenge.

(2) Word Size Limitations

Word size limitations in certain programming languages can be a significant challenge when
implementing data structures like Fusion Trees. These limitations can restrict the number
of bits that can be operated on simultaneously and affect the efficiency of bit manipulation
operations, which are often a crucial part of Fusion Tree algorithms. Dealing with word size
limitations effectively is essential to ensure the data structure functions optimally.

(3) Portability Across Languages

Fusion Trees implemented in one programming language might not be easily portable to another 
language due to language-specific differences in data types, memory management, and other
low-level details. Ensuring that Fusion Trees can be used across different languages while 
maintaining efficiency and functionality can be a challenge.
