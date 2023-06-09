Download Link: https://assignmentchef.com/product/solved-cs261-assignment-1
<br>
<h1>Q0.c</h1>

Write a program (Q0.c) to do the following:

<ol>

 <li>In the main function, declare an integer, <strong>x</strong>. Print the address of <strong>x</strong> (using the address of operator). Pass <strong>x</strong> as an argument to a function <strong>void fooA(int* iptr)</strong>.</li>

 <li>In <strong>fooA(int * iptr)</strong>, print the value of the integer pointed to by <strong>iptr</strong>, the address pointed to by <strong>iptr</strong>, and the address of <strong>iptr</strong></li>

 <li>In the main function, following the call to <strong>fooA(…)</strong>, print the value of <strong>x</strong>.</li>

</ol>

<strong>Scoring:</strong>

Address of <strong>x</strong>

Value of what <strong>iptr</strong> points to

Address pointed to by <strong>iptr</strong>

Address of <strong>iptr</strong> itself

Value of <strong>x</strong>

<h1>Q1.c</h1>

Write a program (Q1.c) in which you consider the following structure:

struct student {        int id;        int score;   };

and the declaration in the main function: struct student *st = 0;

Implement the following functions and demonstrate their functionality by calling them (in the order given) from the main function

<ol>

 <li>Write a function <strong>struct student* allocate()</strong> that allocates memory for ten students and returns the pointer.</li>

 <li>Write a function <strong>void generate(struct student* students)</strong> that generates random IDs and scores for each of the ten students and stores them in the array of students. You can make use of the <strong>rand() </strong>function to generate random numbers. Ensure that IDs are unique and between 1 and 10 (both inclusive) and score is between 0 and 100 (both inclusive).</li>

 <li>Write a function <strong>void output(struct student* students)</strong> that prints the ids and scores of all the students. the output of the function need not to be sorted.</li>

 <li>Write a function <strong>void summary(struct student* students)</strong> that prints the minimum score, maximum score and average score of the ten students.</li>

 <li>Write a function <strong>void deallocate(struct student* stud)</strong> that frees the memory allocated to students. Check that students is not NULL (NULL == 0) before you attempt to free it.</li>

</ol>

<h1>Q2.c</h1>

Write a program (Q2.c) with the following:

<ol>

 <li>a function <strong>int foo(int* a, int *b, int c)</strong> which should perform the following computations

  <ol>

   <li>Set the value of <strong>a</strong> to twice its original value.</li>

   <li>Set the value of <strong>b</strong> to half of its original value.</li>

   <li>Assign <strong>a</strong> + <strong>b</strong> to <strong>c</strong>.</li>

   <li>Return the value of <strong>c</strong></li>

  </ol></li>

 <li>In the main function, declare three integers <strong>x</strong>,<strong>y</strong>, and <strong>z</strong>, and assign them values 5, 6, and 7 respectively. Print the values of <strong>x</strong>,<strong>y</strong>, and <strong>z</strong>. Call <strong>foo(…)</strong> appropriately passing <strong>x</strong>,<strong>y</strong>, and <strong>z</strong> as arguments and print the returned value. After the function call, print out the values of <strong>x</strong>,<strong>y</strong>, and <strong>z </strong> Answer the following question in a comment <strong>at the bottom of the file</strong>: Is the return value different than the value of z? Why?</li>

</ol>

<h1>Q3.c</h1>

Write a function <strong>void sort(int* numbers, int n)</strong> to sort a given array of <strong>n</strong> integers in <strong>ascending order</strong>.

<ol>

 <li>In the main function, declare an integer <strong>n</strong> and assign it a value of 20. Allocate memory for an array of <strong>n</strong> integers using <strong>malloc</strong>. Fill this array with random numbers, using the c math library random number generator <strong>rand()</strong>. Print the contents of the array.</li>

 <li>Pass this array along with <strong>n</strong> to the <strong>sort(…)</strong> function above. Print the contents of the sorted array following the call to <strong>sort(…)</strong>. You may *not* use the C provided sort function (e.g. <strong>qsort()</strong>).</li>

</ol>

<h1>Q4.c</h1>

Consider the structure <strong>student</strong> in Q1.c. Modify the above <strong>sort(…)</strong> function from Q.3 to sort an array of <strong>n </strong>students based on their scores in <strong>ascending order</strong>. The function prototype is <strong>void sort(struct student* students, int n)</strong>. The IDs and scores of the students are to be generated randomly (see use of <strong>rand()</strong>). Also you must make sure that IDs are unique.

<h1>Q5.c</h1>

Write a function <strong>void sticky(char* word)</strong> where word is a single word such as “sticky” or “RANDOM”.

<strong>sticky()</strong> should modify the word to appear with “sticky caps” (http://en.wikipedia.org/wiki/StudlyCaps) , that is, the letters must be in alternating cases(upper and lower), starting with upper case for the first letter. For example, “sticky” becomes “StIcKy” and “RANDOM” becomes “RaNdOm”. Watch out for the end of the string, which is denoted by ‘ ’. You can assume that legal strings are given to the <strong>sticky()</strong> function.

NOTE: You can use the <strong>toUpperCase(…)</strong> and <strong>toLowerCase(…)</strong> functions provided in the skeletal code to change the case of a character. Notice that <strong>toUpperCase()</strong> assumes that the character is currently in lower case. Therefore, you would have to check the case of a character before calling <strong>toUpperCase()</strong>. The same applies for <strong>toLowerCase()</strong>.