## chapter 1
#### motivation
- What are algorithms?
-  Why is the study of algorithms worthwhile?
-  What is the role of algorithms relative to other technologies used in computers?
### 1.1 Algorithms 
Algorithm
: -     a sequence of computational steps that transform input to output. 
   -     a tool for solving a well-specified computational problem
***The problem*** specifies in geniral the desired input/output relationship.
***The Algorithm*** describes a specific computational procedure for achieving that input/output relationship.
***Instance of a problem*** 
-     Input sequence that consists of Input and Constrains (which imposed in the problem ).   
**Algorithm sort is best !!!** it depends on **Factors**
- the number of items to be stored
- what level the items are already somewhat sorted 
- possible restrictions on the item values
- the architecture of the computer
- storage devices to be used 
   - main memory
   -  disks
   -  tapes

**Algorithm is correct if**  for every input instance,
 it halts with the correct output.  

**An incorrect algorithm** 
: - might not halt at all on some input instances, or it might halt with an incorrect answer.
  -  can sometimes be useful, if we can control their error rate.
  - EX) algorithms for finding large prime numbers.

##### what kinds of problems are solved by algorithm ?
- **The Human Genome Project** Identify 100,000 genes in DNA by determining sequence of 3 billion chemical base pairs.
needing sophisticated algorithms to store info in DBs and tools for Data analysis. 
- **Internet** sites on the Internet are able to manage and manipulate large volume of data , finding good routes data will travel by using clever algorithms.
- **Electronic commerce** using numerical algorithms and number theory.
- **Manufacturing** Using linear programming to allocate place to maximize oil company profit.
- **shortest route** number of possible routes in road map can be huge, so modeling road map as a graph helping to find shortest path from one vertex to another in graph. 
- **longest common subsequence** (subsequence is all possible some or all or none elements =2^n )
 To measure how similar two ordered sequences are? using dynamic programming,  you get it.
**Library of Parts Application** each part may include instances of other parts.
we need to list the parts in order to each part apprears before any part that uses it.
assume n parts .so, n! possible orders.
we can not generate each possible order and verify it. solution is in topological sorting.
##### Two common characteristics in algorithmic problems
1. they have many solutions and most of them do not solve it by hand.
2. they have practical applications

Not every problem solved by algorithms has an easily identified set of candidate solutions. 
EX) computing the discrete Fourier transform to samples of signals.
solution : fast fourier transform(FFT). 
### Data Structure
    - way to store and organize data in order to facilitate access and modification.
it is important to
: - know the strengths and limitations of them.
  - learn technique of algorithm design and analysis 

This book is about efficient algorithms (measure of efficiency is speed) but some problems have no efficient solution(**NP-complete**) like 
“traveling-salesman problem”, handeled by **approximation algorithm**
### Parallelism
In order to perform more computations per second, chips designed to contain several “cores”
we need to design algorithms with parallelism in mind **"Multithreaded algorithms"**
( championship chess program)  

### 1.2 Algorithms as a technology
Computing time is a bounded resource, and space in memory.
You should use these resources wisely,so
Algorithms that are efficient in terms of time or space will help you do.

**Efficiency**
Different algorithms solving same problem often differ dramatically in efficiency.
These differences are more significant than differences due to hardware and software.
*Ex)* two sorting algorithms
- **insertion sort**___  c1.n^2 
- **merge sort**  _____    c2.n.log(n)
______________  c1 < c2 
 Although insertion sort runs faster  for small input sizes, once input size n becomes large enough, merge sort becomes faster.
  - sorting 10 million numbers takes 5.5 hours with insersion and 20 minute in merge sort.
  - sorting 100 million numbers takes 23 days with insersion and 4 hours in merge sort. 
  
**Algorithms and other technologies**  
- Algorithms is a technology like computer hardware.

- Total system performance depends on choosing efficient algorithms as on choosing fast hardware.
- **consider a Web-based service that determines how to travel from one location to another.**
Its implementation would rely on
  - fast hardware
  - a graphical user interface
  -  wide-area networking
  - object orientation.
  - algorithms for certain operations, such as
     - finding routes (probably using a shortest-path algorithm)
     - rendering maps
     - interpolating addresses.
     
     
  **In addition to**
  - The hardware design used algorithms
  - The design of any GUI relies on algorithms
  - Routing in networks relies heavily on algorithms
  - compiler, interpreter, or assembler use
  algorithms
  
- Algorithms are at the core of most technologies used in modern computers.
- we use them to solve larger problems than ever before.

Having a solid base of algorithmic knowledge and technique is one characteristic that separates the truly skilled programmers from the novices.
With modern computing technology, you can accomplish some tasks without knowing much about algorithms, but with a good background in algorithms, you can do much, much more .




