# Practice Quiz
## Lesson-1

1. What are the unix commands to create a folder "hello", enter the folder, create a file "hello.txt", then list the contents of the folder "hello"?
2. What is the unix command to edit a file?
3. What is the file extension for a bash script file? a c file?
4. How do you compile a c file? What does compiling a c file mean?
5. What is Github used for? What is version-control?


## Lesson-2

1. What is the difference between an unsigned int and a signed int?
2. How many bits are in a byte?
3. Write the number 19 in binary.
4. Convert 00010011 to decimal.
5. Given the data types: char, int, short, long, float, double, long double.
  	- What data types can store a decimal number?
 	 - What data type is number 3.0f?
 	 - What data type is the number 2L?
6. What does the % operator do? For example, what is the result of 5%2 ?
7. What do the following characters mean?
	  - '\t'
	  - '\n'
	  - '\?'
	  - '\\'


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


 7. Refer to an ASCI chart to answer this question. How can you make the following program output an 'H'?
 ```c
 #include <stdio.h>

int main()
{
    char c = 'C';
    printf("%c", c + 255);
    return 0;
}
```

 8. Fill in the correct format specifiers in the code below where there is a __:
 ```c
 #include <stdio.h>
#include <math.h>
int main()
{
    int i = 4;
    printf("__\n", i);
    
    char c = 'p';
    printf("__\n", c);
    
    float f = 4.5f;
    printf("__\n", f);

    double d = 4.5;
    printf("__\n", castResult);
    
    return 0;
}
```

 9. What is the output of the following expressions?
 	 - 5 < 4
 	 - (4 > 3) && (3 != 9 )
 	 - !((5 < 2) || !(3 < 1))
	 - (2 <= 2) || !(3 < 1)
  
  
  # Lesson-3
  1. What is the output of the following operations? Write out the numbers in binary, and do the operations, then convert the final result back to decimal. Show your work.
  	  - 5 & 4
 	   - 5 | 4
 	   - 5 ^ 4 
 	   - 25 & 11
 	   - 5 << 2
 	   - 15 | 7
 	   - 12 >> 2
 	   - 11 ^ 7

   2. Do the following math with the binary numbers and the decimal numbers. Show your work.
 	   - 10 + 5
 	   - 10 - 5 (Hint: take the two's complement of 5, and add 10 + (-5) to get the answer)
 	   - 12 + 3
	   - 12 - 3
	   - 25 + 1


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

  4. What type of conditional statement (if/else, if/else if/else, while, switch) is best to use in the following situations?
 	   - print out "greater" if the input is greater than 5, otherwise print out "less"
 	   - print "hello" 4 times
 	   - print out the numbers 1-10 each on a new line
	    - for each letter of the alphabet print out an animal that starts with that letter
 	   - Add the numbers, subtract the numbers, divide the numbers based on whether a '+', '/', or '-' was entered into the program


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
``
  
  
