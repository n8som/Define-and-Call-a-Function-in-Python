# Define-and-Call-a-Function-in-Python

<h2>Introduction</h2>

As a security analyst, when writing out Python code to automate a certain task, I often find myself needing to reuse the same block of code more than once. This is why functions are important. I can call that function whenever I need the computer to execute those steps. Python not only has built-in functions that have already been defined but also provides the tools for users to define their functions. Security analysts often define and call functions in Python to automate a series of tasks.

In this lab, I'll practice defining and calling functions in Python.

<h2>Scenario</h2>

Writing functions in Python is a useful skill in my work as a security analyst. In this lab, I'll define and call a function that displays an alert about a potential security issue. Also, I'll work with a list of employee usernames, creating a function that converts the list into one string.

<h2>Task 1</h2>

The following code cell contains a user-defined function named alert().

For this task, analyze the function definition, and make note of my observations.

Note that the cell will not produce an output because the function is just being defined here.

![image](https://github.com/n8som/Define-and-Call-a-Function-in-Python/assets/110139109/bc5a39d8-415f-4c52-948c-cfe68c234865)

This creates a function that outputs, "Potential security issue. Investigate further."

<h2>Task 2</h2>

For this task, call the alert() function that was defined earlier and analyze the output.

![image](https://github.com/n8som/Define-and-Call-a-Function-in-Python/assets/110139109/65ad7791-ca85-449f-b050-f67dea0244ca)

Placing the code in a function allows me to efficiently reuse the code. Whenever I need to display messages about a potential security issue and further investigation, I can just call the alert() function. The alternative would be to write out that print() statement every time, which would be tedious.

<h2>Task 3</h2>

Functions can include other components that I've already worked with. The following code cell contains a variation of the alert() function that now uses a for loop to display the alert message multiple times.

For this task, call the new alert() function and observe the output.

![image](https://github.com/n8som/Define-and-Call-a-Function-in-Python/assets/110139109/0d222b14-bb10-49d6-a4df-63899a1c9d0f)

The difference in behavior from this function compared to the last is due to the for loop used in the second version. This loop iterates over a range of numbers (specified by range(3)) and executes a print() statement in each iteration.

<h2>Task 4</h2>

In the next part of my work, I'm going to work with a list of approved usernames, representing users who can enter a system. I'll be developing a function that helps me convert the list of approved usernames into one big string. Structuring this data differently enables me to work with it in different ways. For example, structuring the usernames as a list allows me to easily add or remove a username from it. In contrast, structuring it as a string allows me to easily place its contents into a text file.

For this task, start defining a function named list_to_string(). Write the function header. Note that running this cell will produce an error since this cell will just contain the function header; I'll write the function body and complete the function definition in a later task.

![image](https://github.com/n8som/Define-and-Call-a-Function-in-Python/assets/110139109/34ccfeb8-53f0-41d3-a55a-d53a63f58981)

<h2>Task 5</h2>

Now I'll begin to develop the body of the list_to_string() function.

In the following code cell, I'm provided a list of approved usernames, stored in a variable named username_list. My task is to complete the body of the list_to_string() function. Recall that the body of a function must be indented. To complete the function body, write a loop that iterates through the elements of the username_list and displays each element. Then, call the function and run the cell to observe what happens.

![image](https://github.com/n8som/Define-and-Call-a-Function-in-Python/assets/110139109/987e9088-530f-4ea2-964b-980806afe34d)

<h2>Task 6</h2>

String concatenation is a powerful concept in coding. It allows me to combine multiple strings to form one large string, using the addition operator (+). Sometimes analysts need to merge individual pieces of data into a single string value. In this task, I'll use string concatenation to modify how the list_to_string() function is defined.

In the following code cell, I'm provided a variable named sum_variable that initially contains an empty string. My task is to use string concatenation to combine the usernames from the username_list and store the result in sum_variable.

In each iteration of the for loop, add the current element of username_list to sum_variable. At the end of the function definition, write a print() statement to display the value of sum_variable at that stage of the process. Then, run the cell to call the list_to_string() function and examine its output.

![image](https://github.com/n8som/Define-and-Call-a-Function-in-Python/assets/110139109/dc65e802-4dc5-4318-b334-0f1cdf9fff51)

The output shows all the elements from username_list merged in one line. In its current format, the output is difficult to read. It's difficult to decipher where one username ends and the next begins.

<h2>Task 7</h2>

In this final task, I'll modify the code I wrote previously to improve the readability of the output.

This time, in the definition of the list_to_string() function, add a comma and a space (", ") after each username. This will prevent all the usernames from running into each other in the output. Adding a comma helps separate one username from the next in the output. Adding a space following the comma as an additional separator between one username and the next makes it easier to read the output. Then, call the function and run the cell to observe the output.

![image](https://github.com/n8som/Define-and-Call-a-Function-in-Python/assets/110139109/f64c897b-f67c-40e9-9712-479bb2561231)

The output shows all the elements from username_list in one line. This time, there's a comma and a space after each username. This format is much easier to read. It's easier to distinguish one username from the next.

<h2>Conclusion</h2>

What are the key takeaways of this lab?

- Python allows me to define and call functions that I create.
- The main components of a function definition header include the function header and the function body.
  - The function header includes the def keyword, followed by the name of the function, followed by parentheses, followed by a colon.
  - The function body includes an indented block of code that instructs the computer on what to do when the function is called.
- String concatenation involves using the addition operator (+) to combine multiple strings.
  - One use case for string concatenation is combining the strings from a list into one large string.


