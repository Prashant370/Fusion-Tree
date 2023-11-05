# CS201project

General instruction
------------------------
How to compile and run the code

(1) check that package is install in linux or other device
(2) gcc file_name.c for compile
(3) ./a.out for run the code

---------------------------------------------------------------

---------------------------------------------------------------
When we compile and run the code in ```fusiontree.cpp``` 
we should 
obtain the following output:

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
---------------------------------------------------------------
##References##
https://stackoverflow.com/questions/3878320/understanding-fusion-trees

https://courses.csail.mit.edu/6.851/fall17/scribe/lec12.pdf

https://web.stanford.edu/class/archive/cs/cs166/cs166.1186/lectures/16/Small16.pdf

https://web.stanford.edu/class/archive/cs/cs166/cs166.1196/lectures/16/Small16.pdf

https://dl.acm.org/doi/pdf/10.5555/139404.139466

https://users.cs.utah.edu/~pandey/courses/cs6968/spring23/papers/fusiontree.pdf

https://youtu.be/xSGorVW8j6Q?si=gw10JReUyE8gNRsH

https://youtu.be/3_o0-zPRQqw?si=BmUlF3DbHXy9KOdQ
--------------------------------------------------------------------
# Fusion Tree
Fusion Tree implementation in C++

This repository contains an implementation of a Fusion
Tree that can perform predecessor queries using a 
constant number of arithmetic operations of a standard 
Integer class in c++.



The ```FusionTree``` class is defined
and is very simple to use. A ```FusionTree``` class 
has the following public methods that can be called by
the user:

```C++
 pair<vector<int>, int> getConst(const std::vector<int>& b_bits)
```

```C++
 int getMask(const std::vector<int>& mask_bits)
```


```C++
void initiateNode(Node* node)
```
initate the tree

```C++
int sketchApprox(Node* node, int x)
```
```C++
void splitChild(Node* node, int x)
```
```C++
int parallelComp(Node* node, int k)
```
```C++
int predecessor(int k, Node* node = nullptr)
```
```C++
int successor(int k, Node* node=nullptr)
```





## Example

Although its implementation can be quite complicated, 
using it is fairly simple and relies only on its four
public methods. In our repository, the file 
fusiontree.cpp can be found and contains a
brief example of how to construct and query a 
```fusiontree```. Its main function can be seen below:



A brief explanation of the example code and its output
can be seen below:




In line 16, we use the ```fusiontree``` constructor to
create an instance of a ```fusiontree``` using the 
environment constants defined by `````*env````` that 
contains the elements in ```small_squares```.

```C++
fusiontree my_fusiontree(small_squares, env);
```
In lines 571-576, 
```C++
    int idx1 = ft.predecessor(3);
    int idx2 = ft.predecessor(16);
    int idx3 = ft.predecessor(0);
    int idx4 = ft.successor(0);
    int idx5 = ft.predecessor(10);

```


