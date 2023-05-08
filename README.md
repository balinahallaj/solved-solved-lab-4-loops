Download Link: https://assignmentchef.com/product/solved-solved-lab-4-loops
<br>
1) There is a famous story about a primary school teacher who wanted to occupy his studentsâ€&#x2122; time by making the children compute the sum of 1 + 2 + 3 + â€¦ + 100 by hand. As the story goes, the teacher was astounded when one of the children immediately produced the correct answer: 5050. The student, a child prodigy, was Carl Gauss, who grew up to be one of the most famous mathematicians of the eighteenth century. Repeat Gaussâ€&#x2122;s remarkable calculation by writing a loop that will compute and print the above sum. After you have the program working, rewrite it so you can compute 1 + 2 + â€¦ + n where n is any positive integer.

Using the code shown below, complete the while loop to compute the sum.

“`javapublic class WhileLoop{public static void main(String[] args){int sum = 0;int i = 1;int n = 100;while ( ) // Complete the condition{// Add code to compute the sum}System.out.println(“The sum of 1 + 2 + … + ” + n + ” is ” + sum);}}“`

2) Java provides three types of loops: while, for, and do (also called do-while). Theoretically, they are interchangeable â€“ any program you write with one kind of loop could be rewritten using any of the other types of loops. As a practical matter, though, it is often the case that choosing the right kind of loop will make your code easier to produce, debug, and read. It takes time and experience to learn to make the best loop choice, so this is an exercise to give you some of that experience.

Repeat the exercise again but this time using a for loop. Which form of loop seems to work best? Why?

“`javapublic class ForLoop{public static void main(String[] args){int sum = 0;int i = 1;int n = 100;for ( ) // Complete the for loop{// Add code to compute the sum}System.out.println(“The sum of 1 + 2 + … + ” + n + ” is ” + sum);}}“`

3) A do-while loop is most appropriate when the condition for repeating the loop statements is not known in advance, i.e., it is determined in the loop. Write a program that uses a while loop. In the following program, each iteration of the loop prompts the user to enter a number â€“ positive, negative, or zero in order to keep a running total of the numbers the entered and also keep a count of the number of entries the user makes. The program should stop whenever the user enters â€œQâ€ to quit. When the user has finished, it prints the grand total and the number of entries the user typed.

Because any number can be entered, we need to have another indication of whether or not the user has entered a number or a â€œQâ€. There are two ways to accomplish this task:1) read the input using the Scanner next() method checking to see if is a number of a â€œQâ€-or-2) check to see if the user has entered a number with the Scanner hasNextDouble() method. Choose one approach and complete the code shown below.

“`javaimport java.util.Scanner;

public class DoWhile{public static void main(String[] args){double total = 0;int count = 0;double inputValue;Scanner in = new Scanner(System.in);do{inputValue = in.nextDouble();total = total + inputValue;count = count + 1;System.out.println(“Enter a number or type ‘Q’ to Quit”);} while ( );System.out.println(“The total was ” + total + “.”);System.out.println(“You typed ” + count + ” values.”);}}“`