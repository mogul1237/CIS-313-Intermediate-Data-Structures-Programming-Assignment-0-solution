# CIS-313-Intermediate-Data-Structures-Programming-Assignment-0-solution

Download Here: [CIS 313, Intermediate Data Structures Programming Assignment 0 solution](https://jarviscodinghub.com/assignment/cis-313-intermediate-data-structures-programming-assignment-0-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

Problem 1. System Tools Warmup
This problem will let you practice with some essential system utilities.
Before you start, you will need to set up a CIS Department systems account (if you don’t already have one). You can stop by the department oﬃce in Deschutes Hall or use the following self-service link:
https://systems.cs.uoregon.edu/wiki/index.php?n=Help.Account
Reference the Lab 1 Notes for the terminal commands needed to complete this problem.
Log onto ix-dev and create a new directory named CIS313. Inside that directory create another directory named pset0. Go into the CIS313/pset0 directory and copy the instructions for this problem, given by the following path, into your current directory:
/home/users/hampton2/lab1 313/instructions
Alternately, you can download the instructions from the following link:
https://ix.cs.uoregon.edu/~hampton2/313/instructions
View the contents of the instructions ﬁle to complete this problem.
2
Problem 2. I/O Warmup
Download the Programming Assignment 0 starter pack here:
https://ix.cs.uoregon.edu/~hampton2/313/proj0_starter.tar
Unpack it with the tar command (reference the Lab 1 Notes for help if needed).
The starter pack contains two Python 3 ﬁles: a Calculator class and a driver program. You won’t be required to use Python to complete the course assignments, but it’s strongly encouraged! Python is a great language to know right now for succeeding with tech interviews.
The calculator class has already been written for you. It implements the following (public) methods:
add(X): Takes a single integer argument and adds it to the running total. Should be amortized O(1) time.
mult(X): Takes a single integer argument and multiplies the running total by X. Should be amortized O(1) time.
seen(X): Takes a single integer argument and returns a boolean indicating whether the running total has ever been equal to X. Should be amortized O(1) time.
The driver program has also already been written for you! It takes a single command-line argument, which will be a ﬁlename. The input ﬁle will contain instructions for calculator operations. The ﬁrst line of the input ﬁle will be an integer 1 ≤ N ≤ 103 giving the number of instructions. Following will be N lines, each containing an instruction. The possible instructions are: plus X, where −106 ≤ X ≤ 106 is an integer: For this instruction, add X to the running total. Output the running total. times X, where 0 ≤ X ≤ 103 is an integer: For this instruction, multiply the running total by X. Output the running total. seen X, where −107 ≤ X ≤ 107 is an integer: For this instruction, give an indication of whether the running total has ever been equal to X. Output YES if the running total has ever been equal to the given value, else output NO.
All output should be to STDOUT. Each piece of output should be separated by a newline.
Example input ﬁle:
9 times 200 plus 1 plus 2 seen 5 seen 0 times 5 seen 5 seen 3 seen 15
Example output:
3
0 1 3 NO YES 15 NO YES YES
The starter pack also includes sample input and output ﬁles. Your programming assignments will be graded on ix-dev, so you want to be sure that your code works on there. Send your source ﬁles over to ix-dev (e.g., using the scp command) and run them there. The Python 3 interpreter on ix-dev is invoked as python3.
There is a system utility called diff that is super helpful for seeing if two ﬁles match. The diff utility will even catch whitespace diﬀerences that are easy to miss.
It’s often convenient to save the output from a program to a ﬁle. We can do that with the redirection operator:
python3 driver.py sample.input > my output
Note that ﬁle extensions (such as .txt) aren’t as strict on a UNIX-like system as they are on, say, Windows. We can typically use whatever extensions we want. If you want the system to tell you what kind of ﬁle you’ve got, use the file utility:
file my output
Now, let’s compare my output and sample.output:
diff my output sample.output
If you run the diff command and don’t see anything in the terminal, that means it was a perfect match! You’ll notice, however, that we don’t have a perfect match. Use a reference to help you learn how to read the results of diff.
The Calculator class and driver class were implemented for you, but there are two bugs that need to be ﬁxed! The bugs were caught during code review, so read the ﬁles and implement the two ﬁxes that are suggested in the comments.
Once you’ve got a solution that produces a perfect match according to diff, you’re done with this problem.
[Just for fun: if you just want to compare the output of a program with a ﬁle, it’s not necessary to create a temporary ﬁle. The pipe operator allows you to use the output from one command as the input to another command:
python3 driver.py sample.input | diff – sample.output
This is just a brief intro to UNIX system utilities. Learning to use these tools to automate system jobs will save you a lot of time down the road!]
4
Problem 3. Submit Warmup
In this problem, you’ll get practice bundling your submission into a tar ﬁle and uploading it to Canvas.
Navigate to your CIS313/pset0 directory on ix-dev. Create a new directory called submit.
Copy into this new directory (either from elsewhere on ix-dev or from your personal computer) everything that you need to turn in. For this assignment, it’s the following ﬁles:
problem1_solution calculator.py driver.py
It’s a good idea to go through the steps from Problem 2 to test your solution again. It’s easy to avoid accidentally submitting the wrong ﬁles.
Once you’re sure you’ve got the correct ﬁles, write a README for your project. Remember, you can use the following command to create a new ﬁle called README and open it in the nano editor (feel free to use a diﬀerent editor if you prefer):
nano README
Your README should contain your name and exact commands that can be invoked on ix-dev to run your solution for each problem. If your solution takes an input ﬁle, just use a dummy name. For example, your README for this project should look something like this:
Andrew Hampton
Problem 2: python3 driver.py some.input
If you use a language that requires compilation, your README should also include the exact commands to build your project on ix-dev.
Finally, create a tar ﬁle that contains everything you want to submit. In the ﬁlename lastname.tar, replace lastname with your last name:
tar cvf lastname.tar problem1 solution calculator.py driver.py README
You can check that the ﬁle you’ve created is actually a tar ﬁle by using the file command:
file lastname.tar
Now, just copy the tar ﬁle back to your personal computer and upload it to Canvas for Programming Assignment 0.
This is how you will turn in all of the programming projects for this course (and most of your upper division CIS courses). It’s important to follow these instructions because it allows parts of the grading process to be automated. You will lose a substantial amount of credit for an assignment if you don’t follow the submission guidelines or submit the wrong ﬁles.
