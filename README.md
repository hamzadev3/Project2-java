Project requirements: 
Improving on the Word Game
Add the following improvements to the word game. (1) The first letter of the subject letters (the first line
of the input file) must be contained in all the correct guessed words. (2) If a guessed word contains ALL
of the subject letters, that is worth 3 points. (3) Display the correctly guessed words in alphabetical
order.

Lists of Words
Create a class called WordNode which has fields for the data (a Word) and next (WordNode) instance
variables. Include a one-argument constructor which takes a Word as a parameter. (For hints, see the
PowerPoint on "Static vs. Dynamic Structures”.)
public WordNode (Word w) { . . }

Winning the Game
Let the player know if he or she won the game by guessing all the words on the solutions list. Show a
MessageDialog in this case, and ask the user if he or she would like to play again.
Create a File Menu in your GUI
Add a file menu to your game GUI with options to open any file for reading (and processing the file as in
Project 2), and one to Quit the program. You will need a FileMenuHandler class to handle the events
from the FileMenu. Be sure to use getAbsolutePath() when getting the file from the JFileChooser, not
getName().

Handle Exceptions
Create an exception called IllegalWordException (by extending IlegalArgumentException as shown in
lecture) and have the constructor of the Word throw it. A Word is illegal if it doesn’t contain all lowercase letters. Use a try/catch statement to catch this exception in your program, and show the erroneous
Words in the console. A data file will be provided that has illegal words in it.
