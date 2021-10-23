# ECE361-HW2
ECE 361 Fall 2021
Homework #2
THIS ASSIGNMENT SHOULD BE SUBMITTED TO D2L BY 10:00 PM ON SUN, 24-OCT-2021. THERE IS NO “GRACE PERIOD” FOR THIS ASSIGNMENT AND NO LATE ASSIGNMENTS WILL BE ACCEPTED AFTER 7:00 AM ON MON, 25-OCT BECAUSE I AM PLANNING TO REVIEW THE SOLUTION IN CLASS ON MONDAY.
THE ASSIGNMENT IS WORTH 100 POINTS. IT IS EASIEST TO GRADE, AND I BELIEVE EASIEST FOR YOU TO SUBMIT, SOURCE CODE FILES AS TEXT FILES INSTEAD OF CUT/PASTE YOUR CODE INTO A .doc OR .docx FILE. SHORT ANSWER, TRUE/FALSE AND MULTIPLE-CHOICE QUESTIONS SHOULD BE SUBMITTED IN A SINGLE TEXT OR .PDF FILE FOR THE ASSIGNMENT. CLEARLY NAME THE FILES SO THAT WE KNOW WHICH QUESTION THE ANSWER REFERS TO. SUBMIT THE PACKAGE AS A SINGLE .ZIP OR .RAR FILE (EX: ece361f21_rkravitz_hw2.zip) TO YOUR D2L HOMEWORK #2DROPBOX.
YOU MAY OPTIONALLY USE GIT AND GITHUB TO MANAGE THIS ASSIGNMENT BUT, IF YOU DO, PLEASE SAVE/DOWNLOAD A .ZIP OF YOUR FINAL REPOSITORY TO YOUR D2L HOMEWORK #2 DROPBOX. I STRONGLY SUGGEST THAT YOU DO SO – USING GIT AND GITHUB FOR YOUR ASSIGNMENTS WILL NOT BE OPTIONAL GOING FORWARD.
Problem 1 (30 pts): Writing and compiling C using gcc on the command line
a. (15 pts) Write an application in C that reads integers from the console into a 5 x 5 array and then prints the row sums and the column sums. For example:
Enter row 1: 8 3 9 0 10
Enter row 2: 3 5 17 1 1
Enter row 3: 2 8 6 23 1
Enter row 4: 15 7 3 2 9
Enter row 5: 6 14 2 6 0
Row totals: 30 27 40 36 28
Column totals: 34 37 37 32 21
b. (10 pts) Compile and execute your application using the gcc command line. Include the source code and a console transcript (.txt file) including the terminal output from a test case of your choosing.
c. (5 pts) What is the Big O() for the algorithm that sums the rows and columns in your application? Explain why. You do not need to include the code that fills the array from the user input in your calculation.
Problem 2 (30 pts): Recursion
a. (8 pts) Genghis Khan organized his men into groups of 10 soldiers under a “leader of 10” (10 soldiers + 1 leader). Ten “leaders of 10” were under a “leader of 100.” Ten “leaders of 100” were under a “leader of 1000.”
1) If Khan had an army of 10,000 soldiers at the lowest level, how many men in total were under him in his organization? Show your work.
2) If Khan had an army of 5763 soldiers at the lowest level, how many men in total were under him in his organization? Assume that the groups of 10 should contain 10 soldiers, but that one group at each level may need to contain fewer. Show your work.
b. (12 pts) Write a C function:
float maximum(float list[], int n);
that recursively finds the largest floating point number between list[0] and list[n -1]. Assume at least one element is in the list. n is the number of floating point numbers in the list[] array.
c. (10 pts) Compile and execute the source code for your maximum() function and the test_maximum.c program included in starter_files/prob2 folder. Include your source code, source code for the test program if you changed it, and a console transcript (.txt file) of your output.
Problem 3 (40 pts): A Singly Linked List ADT
While I generally like and appreciate Karumanchi’s approach to ADTs, I do not feel that Karumanchi’s implementation of his singly linked list code is a good example of an Abstract Data Type (ADT). Chief amongst my complaints is that Karumanchi’s algorithm creates the head pointer in main() rather than implementing a createList() function in the ADT. As a result, the solution exposes details of the ADT that could have been hidden.
Fortunately, I feel that Karumanchi redeemed himself with his code examples for Stacks (Chapter 4) and Queues (Chapter 5) by implementing create functionality and hiding the implementation details. Now you have a chance to do the same for a linked list ADT.
a. (10 pts) Refactor Karumanchi’s SinglyLinkedList.c to separate the linked list ADT and main() into two files. Create a header (.h) file for your newly minted linked list ADT. The original code is included in the starter_files/prob3 folder for this assignment. Hint: there is no main() in Karumanchi’s code. The function SinglyLinkedList_test() can be used as a simple test by either renaming it main() or adding a main() that displays a greeting and calls SinglyLinkeList_test().
b. (15pts) Rewrite the code in SinglyLinkedList.c to bring the declaration/creation of the head pointer of the list into the ADT. Consider adapting the approach that Karumanchi used in his Stack and Queue examples, or you may choose to include an array of head pointers in the ADT, returning an index into that array whenever a new linked list (not a node…a new linked list) is created. Your ADT should return an indication of whether the list was created successfully (ex: a NULL pointer or an illegal index like -1 if the create list functionality failed).
c. (15 pts) Rewrite main()to use your new ADT. Compile and execute the program. Include your source code and a console transcript (.txt file) showing that your new ADT works.
