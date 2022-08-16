# The Art of Computer Programming, vol 1, chap 1

Author:: Donald E. Knuth
Date Created:: 2021-12-21
- - - 

### Algorithms
The word “Algorithm”, was initially called *algorism*, which meant the process of doing arithmetic using **Arabic Numerals**. 
By 1950, the word algorithm as most frequently associated with **Euclid’s algorithm**,  a process for finding the greatest common divisor of two numbers.

![[Screen Shot 2021-12-22 at 8.30.09 AM.png]]
Each step of an algorithm begins with a phrase in brackets that sums up as briefly as possible the principal content of that step. It also usually appears in an accompanying *flow chart*. 

![[Screen Shot 2021-12-22 at 12.16.56 PM.png]]
Parenthesized comments give more information to the reader about the variables or current goals of the algorithm. 
The ← in step **E3** is called the *replacement* operation. It is sometimes called *assignment* or *substitution*. m ← n means that the value of m is replaced by the current value of n.

Keep in mind that there is a difference between using the *equality* operator and the *replacement* operator. The replacement operator changes the value of one variable to another while the equality operator compares two operands. 
$$
m\leftarrow n \ne m=n
$$
The operation of *increasing n by 1* is given as “n ← n + 1”. This means that the next value of n is would be given as the next value of n. If assigning two variables the same value, we can write:
$$n\leftarrow m \leftarrow r$$
To interchange two values, we can write $m \leftrightarrow n$. This operation can be written using a new variable $t$:
$$t \leftarrow m,\ m \leftarrow n,\ n \leftarrow t$$
The heavy vertical line at the end of step **E3** is used to indicate the end of an algorithm and the resumption of text.

Imagine a scenario where $m$ < $n$, the algorithm divides $m$ by $n$ giving a quotient of 0 and a remainder of $n$. Then the algorithm assigns $n$ to $m$ [$m \leftarrow n$] and then $n \leftarrow r$. This leads to the algorithm proceeding to interchange $m$ and $n$. We could solve this by inserting a new step at the beginning:

![[Screen Shot 2021-12-22 at 2.24.00 PM.png]]
Adding this would make no essential change in the algorithm, except increase its length slightly, and decrease its running time in about one half of all cases.

There are 5 important features of an algorithm:
1. **Finiteness** → An algorithm must always terminate after a finite number of steps.
2. **Definiteness** → Each step of an algorithm must be precisely defined.
3. **Input** → An algorithm has zero or more inputs.
4. **Output** → An algorithm has one or more outputs.
5. **Effectiveness** → Algorithms must be effective in their opperations.

A procedure that has all of the characteristics of an algorithm except that it possibly lacks finiteness may be called a **computational method**. Another nonterminating computational method is a **reactive process**, which continually interacts with its environment.

A **program** is an expression of a computational method in a computer language.