# CS50’s Introduction to Computer Science, Week 0

Author: Harvard University
Date Created: 2021-12-21
- - - 

### Number Systems, Characters & ASCII
Binary Numbers are made up of binary digits (1’s and 0’s) which are called **bits** (Binary Digits). These **bits** set the stage for how much bytes, kilobytes, megabytes etc, a computer can store. ^654627

The hexadecimal number system is made up of numbers 1 through 9 and 10 through 15 being represented as letters of the alphabet e.g A → 10, F → 15
	
**ASCII** →* American Standard Code for Information Interchange*. This is a mapping of letters and characters to numbers.
- Characters are made using *8-bits*
	- 8-bits make up a *byte*
	- $2^8$ characters can be made from 8-bits
	- Emoji’s are made up of bits too.

Using 8-bits does not provide enough character possibilities, so more bits can be used such as 16-bits, 32-bits and 64-bits to represent a vast amount of characters from different languages to symbols and emoji’s. For example the binary representation of the laughing emoji 😂 is 0000000111111011000000010
 
**File extensions** e.g (.jpeg, .png, .csv, .mp3), contextualize bits of information. It classifies the information or data being represented by the bits. For example the bits used in a .mp4 video, represent the change in RGB value in the video. The file extension has contextualized the bits to represent the change in RGB values of the video.

### Algorithms 
**Algorithms** are step by step instructions which perform a task or solve a problem. Writing Efficient and Accurate Algorithms are key when solving problems.
* If given a task to find the phone number of a person alphabetically in a phone book, using their name. Several approaches or algorithms can be used to perform this task:
	* You could search each individual page one by one from the beginning of the phone book until you get to the name of the person your searching for. let’s call this $n$.
	* You could alternatively increase the amount of pages you flip through to two pages per flip. e.g pg 1 → pg 3 → pg 5 . . . We’ll call this $n/2$
	* Finally you could start from some arbitrary middle point, and halve the search space by getting rid of the side of the phone book that does not have the first letter of the name your looking for. Let’s call this $\log_2 n$ 

![[Screen Shot 2021-12-21 at 11.13.56 AM.png]]

We can see the time taken by the third algorithm is significantly less than the time taken by the previous algorithms. It is **logarithmic** in terms of time complexity. This is essentially the ideal aim for algorithms in computer science.

### Pseudocode
This is a verbal representation of an algorithm which makes planning easier. The pseudocode of the previous logarithmic algorithm can be given as:

![[Screen Shot 2021-12-21 at 11.24.14 AM.png]]

Some lines above start with statements which are known as **functions**. Functions are **"self contained" modules of code that accomplish a specific task**. The *If* and *Else If* on some lines are called **conditionals**.