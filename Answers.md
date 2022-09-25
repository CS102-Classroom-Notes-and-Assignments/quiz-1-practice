# Practice Quiz
## Lesson-1

1. What are the unix commands to create a folder "hello", enter the folder, create a file "hello.txt", then list the contents of the folder "hello"?
```
mkdir hello
cd hello
touch hello.txt
ls hello
```
2. What is the unix command to edit a file?
```vim```
3. What is the file extension for a bash script file? a c file?
```
bash script - .sh
c file - .c
```
4. How do you compile a c file? What does compiling a c file mean?
```
gcc <file_name>, example: gcc hello.txt
Compiling converts the source code file (the .c file written in the c programming language) into an executable file. The executable file contains machine code (a sequence of 1s and 0s) that can control the CPU of the computer. C is a compiled language, not interpreted, so the source code must be compiled in order for them to be executed. 
```
5. What is Github used for? What is version-control?
```
https://kinsta.com/knowledgebase/what-is-github/ : 
**GitHub** is a website and cloud-based service that helps developers store and manage their code, as well as track and control changes to their code. 

**Version control** helps developers track and manage changes to a software project’s code. As a software project grows, version control becomes essential. Take WordPress… At this point, WordPress is a pretty big project. If a core developer wanted to work on one specific part of the WordPress codebase, it wouldn’t be safe or efficient to have them directly edit the “official” source code.
Instead, version control lets developers safely work through branching and merging.

With branching, a developer duplicates part of the source code (called the repository). The developer can then safely make changes to that part of the code without affecting the rest of the project.

Then, once the developer gets his or her part of the code working properly, he or she can merge that code back into the main source code to make it official.

All of these changes are then tracked and can be reverted if need be.
```

## Lesson-2

1. What is the difference between an unsigned int and a signed int?
```
An unsigned int is an int that can only be positive. A signed in is an integer than can be negative. 
An unsigned int does not need a bit to indicate whether the number is positive or negative, and therefore has a higher range of positive values it can be. On the other hand, a signed integer uses a bit to indicate whether its positive or negative, so it has a lower positive range in exchange for being able to store negative values.
```
2. How many bits are in a byte?
```8```
3. Write the number 19 in binary.
```10011```
4. Convert the binary number 00010011 in decimal.
```19```
5. Given the data types: char, int, short, long, float, double, long double.
  	- What data types can store a decimal number? ```float, double, long double```
 	 - What data type is number 3.0f? ```float```
 	 - What data type is the number 2L? ```long```

6. What does the % operator do? For example, what is the result of 5%2 ?
```modulo operator, 1```
7. What do the following characters mean?
	  - '\t' ```tab```
	  - '\n' ```new line```


6. What is the output of the following program? How might you add precision to the output?
```c
#include <stdio.h>

int main()
{
    float f = 1.5f;
    int i = 3;
    int result = i + f;
    printf("%d", result);

    return 0;
}
```
```
This program outputs 4. You would add precision to the output by making the result a float, as well as changing the %d to %f.
```

 7. Refer to an ASCII chart to answer this question. How can you make the following program output an 'H'?
 ```c
 #include <stdio.h>

int main()
{
    char c = 'C';
    printf("%c", c + 255);
    return 0;
}
```

```
Change the 255 to 5.
```
 8. Fill in the correct format specifiers in the code below where there is a __:
 ```c
#include <stdio.h>
#include <math.h>
int main()
{
    int i = 4;
    printf("%d\n", i);

    char c = 'p';
    printf("%c\n", c);

    float f = 4.5f;
    printf("%f\n", f);

    double d = 4.5;
    printf("%lf\n", d);

    return 0;
}
```

```Blanks filled in above```


 9. What is the output of the following expressions?
 	 - 5 < 4 ```false```
 	 - (4 > 3) && (3 != 9 ) ```true```
 	 - !((5 < 2) || !(3 < 1)) ```false```
	 - (2 <= 2) || !(3 < 1) ```true```
  
  
  # Lesson-3
  1. What is the output of the following operations? Write out the numbers in binary, do the operations, then convert the final result back to decimal. Show your work.
 
 5 & 4 
 ```
 0101
 0100
 -----
 0100 = 4
 ```
 5 | 4
 ```
 0101
 0100
 -----
 0101 = 5
 ```
 5 ^ 4 
 ```
 0101
 0100
 -----
 0001 = 5
 ```	   
 25 & 11
 ```
11001
01011
 -----
01001  = 9
 ```
 5 << 2
  ```
 000101 = 5
 010100 = 5 << 2 = 20
 ```
15 | 7
  ```
 000101 = 5
 010100 = 5 << 2 = 20
 ```
 12 >> 2
  ```
 1100 = 12
 0011 = 12 >> 2 = 3
 ```
 11 ^ 7
  ```
 1011
 0111
 ------
 1100 = 12
 ```
 
   2. Do the following math with the binary numbers and the decimal numbers. Show your work.
10 + 5
```
1010 =10
+
0101 = 5
----
1111 = 15
```
10 - 5 (Hint: take the two's complement of 5, and add 10 + (-5) to get the answer)
```
1010 = 10
+
1011 = -5 (two's complement of 5 = (ones complement of 5) + 1 = 1010 + 1 = 1011)
----
0101 = 5
```
12 + 3
```
1100 =12
+
0011 = 3
----
1111 = 15
```
12 - 3
```
1100 = 12
+
1101 = -3 (two's complement of 3 = (ones complement of 3) + 1 = 1100 + 1 = 1101)
----
1001 = 9
```
25 + 1
```
11001 =25
+
00001 = 1
----
11010 = 26
```

   3. What is the difference between a prefix and a postfix operator? What does the code below print out?
   ```c
   #include <stdio.h>
int main()
{
    int var1 = 5, var2 = 5;
    printf("var1: %d\n", var1);
    printf("var1 postfix increment: %d\n", var1++);
    printf("var1:%d\n", var1);
    printf("------------------\n");
    printf("var2: %d\n", var2);
    printf("var2 prefix increment: %d\n", ++var2);
    printf("var2: %d\n", var2);

    return 0;
}
```
```
++n or --n is prefix, while n++ and n-- is postfix.
++n increments n before its value is used, while n++ increments n after its value has been used.

The program above outputs:
var1: 5
var1 postfix increment: 5
var1:6
------------------
var2: 5
var2 prefix increment: 6
var2: 6
```
  4. What type of conditional statement (if/else, if/else if/else, while, switch) is best to use in the following situations?
 	   - print out "greater" if the input is greater than 5, otherwise print out "less" ```if/else```
 	   - print "hello" 4 times ```while```
 	   - print out the numbers 1-10 each on a new line ```while```
	    - for each letter of the alphabet print out an animal that starts with that letter ```switch```
 	   - Add the numbers, subtract the numbers, divide the numbers based on whether a '+', '/', or '-' was entered into the program ```switch or if/else if/else if/else```


  5. What does the following program do? What does EOF mean?
  ```c
  #include <stdio.h>
main()
{
	int c;
	
	c = getchar();
	while( c != EOF) {
		putchar(c);
		c = getchar();
	}
}
```
  
  
```
The program reads input passed into the executable file. The input can be passed into the file by running "a.out < inputfile.txt". EOF means end of file. This program uses getchar() to get each char value from the inputfile, then print the char, then get the next char value from the input file. This process repeats until the EOF character is reached, meaning its the end of the file.
```
