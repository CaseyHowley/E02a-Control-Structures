
# E02a-Control-Structures

Questions & Answers:

- Q1: Open main01.py. Before running it, what do you expect this program to do?
  - Now right click on the main1.py window and select “Run Python File in Terminal”. Click in the bottom panel, and answer the question. Describe what happened.
  - What do you think the program did with what you typed in answer to the question?

- A1: Before Running, I expect the program to print 'Greetings!' and ask for input (which will not be used).
  - The program run as expected (see above).
  - The program didn't do anything with the input.

- Q2: Open main02.py. Before running it, describe how this is different than main01.py.
  - What do you think the color = input() will do?
  - Run the program in the terminal and answer the question. Did the program do what you expected?

- A2: main02.py actually assigns the input to a variable, and then uses that variable.
  - It should assign the value input to the variable color
  - Yes, the program did what I expected.

- Q3: Open main03.py. Before running it, describe how this is different than main02.py.
  - What is happening on lines 9–12?
  - Why are lines 10 and 12 indented?
  - Run the program and answer the question. What happens if you don’t capitalize Red?
  - What does this tell you about "color"?

- A3: main03.py actually validates the question posed in the input, and returns responses if the question was correctly answered or not.
  - Lines 9-12 are an if/else statement. Some code is executed, depending upon if the input matches the correct answer.
  - Lines 10 and 12 are indented so that they can be properly read (and executed) by the if/else conditionals.
  - If you don't capitalize Red, the statement returns false.
  - This tells us that the variable "color" stores case, as well as content.

- Q4: Open main04.py. Before running it, describe how this is different than main03.py.
  - What problem is this trying to solve?
  - Run the program and answer the question. What happens if you use some other capitalization scheme (i.e., “RED” or “reD“)?

- A4: main04.py is nearly identical, but has an 'or' statement in the conditional, meaning (in this case) two answers will result in the satement being True.
  - This is trying to fix the case sensitivity issue from main03.py.
  - If you use a different capitalization scheme (such as "ReD"), the conditional statement returns false.

- Q5: Open main05.py. What do you expect line 9 to do?
  - What problem is it trying to solve?
  - Run the program and answer the question. What happens if you add spaces before or after the word (i.e., “ RED “ or “ red”)?

- A5: I expect line 9 to convert the variable "color" to lowercase before processing it into the conditional.
  - This is (again) trying to fix the case sensitivity issue from the previous files.
  - Adding spaces before or after the word causes the conditional to return false.

- Q6: Open main06.py. How is line 9 different than in main05.py?
  - What would you guess .strip() is doing?
  - Run the program and answer the question. Is there another way of writing “red” that will break this logic?

- A6: Line 9 now has an added .strip() function applied.
  - I would guess that .strip() isolates the text input, to prevent " red " or similar variations from returning false.
  - Writing it "r e d" will break the program logic and cause it to return false.

- Q7: Open main07.py. Before running this program, how do you expect this to be different than main06.py?
  - What is happening on line 12?
  - Run the program and answer the question.

- A7: main07.py has an elseif conditional, which provides another possible output, in this case if the input is 'pink'.
  - Line 12 is, as mentioned above, and elseif conditional, which is checked if the original if statement fails. It provides another possible output for the conditonal as a whole.

- Q8: Open main08.py. What is the purpose of line 9?
  - Why are lines 10–17 indented?
  - Run the program. What would happen if line 10 were moved before line 9 (and no longer indented)?
  - Make that change and run the program again. (To end any Python program, you can type ctrl-c)

- A8: Line 9 is a while statement, and will repeat until the sequence is broken.
  - Lines 10-17 are indented so that they can be properly read (and executed) by the while statement.
  - If line 10 were before line 9, the while statement may either be avoided entirely, or become an infinite loop.

- Q9: Open main09.py. What is happening on line 13?
  - What is the purpose of “count”?
  - What is happening on line 22?
  - Run the program.

- A9: Line 13 is adding 1 to the variable 'count'
  - 'count' is a count of how many times the user guessed before guessing the right color
  - Line 21 (there is no line 22) is outputting how many times the user guessed.

- Q10: *Extra credit:* open main10.py. Add a comment to each line describing what it is doing (a comment follows a pound sign [#]).
- Q11: *Extra credit:* open main11.py. What is happening on lines 6-11?

- A11: Lines 6-11 are defining a function, chose_color, with the argument (last_color).
  - In the function is a list of colors. Variable c is randomly assigned one of the colors from that list.
  - While the color in variable c matches the last_color argument, c is randomly assigned a new color from the list
  - the color in variable c is then returned