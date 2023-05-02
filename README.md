Download Link: https://assignmentchef.com/product/solved-cmsc202-project-1-fifteen-game-assignment
<br>
<span style="font-size: 2.61792em; letter-spacing: -1px; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen-Sans, Ubuntu, Cantarell, 'Helvetica Neue', sans-serif;">1.   Overview</span>

In this project, you will:

<ul>

 <li>Practice basic C++ syntax including branching structures</li>

 <li>Write a program that calls multiple functions</li>

 <li>Manage a two-dimensional array</li>

 <li>Use simple file input/output</li>

</ul>

<h1>2.   Background</h1>

The fifteen (15 or 16 puzzle) is a common sliding puzzle that you may remember from your youth. It involves a frame of numbered square tiles in random order with one tile missing. The object of the puzzle is to place the tiles in order by making sliding moves that use the empty space.

<strong>Figure 1. Solved 15 Puzzle</strong>

For this effort, we are going to create a game board that the user can manipulate in order to get a board that is out of order into a correct order. Additionally, the game will indicate when the game is “solved” by putting the tiles into the correct location.

The game board will be represented by a two-dimensional grid. The actual implementation of how you want to create the grid is up to your design decisions, but you must meet all requirements listed below for full points.

The user will be able to “slide” any tile to an empty location. If the user tries to slide the tile into a location that is already populated or off of the board, the system will indicate that it is not possible. While we can make the grid of any size, we will start with a standard 4 by 4.

<strong>Figure 2. Sample Grid</strong>

<h1>3.   Assignment Description</h1>

Your assignment is to develop the fifteen game (using text) where the user tries to put each of the tiles into order. On each turn, the user can slide any tile adjacent to a blank into the blank location.

The game continues until all fifteen tiles are in order as shown in figure 1 above. It should then prompt the user for another game.




<h1>4.   Requirements:</h1>

This is a list of the requirements of this application. For this project, it is up to you exactly how you want to implement it. For you to earn all the points, however, you will need to meet all the defined requirements.

<ul>

 <li>You must follow the coding standard as defined in the CMSC 202 coding standards (found on Blackboard under course materials). This includes comments as required.</li>

 <li>The project must be turned in on time by the deadline listed above.</li>

 <li>The project must be completed in C++. You may not use any libraries or data structures that we have not learned in class. These are the only libraries that you are allowed to use in this project <strong>&lt;iostream&gt;, &lt;ctime&gt;, &lt;fstream&gt;, &lt;iomanip&gt;, &lt;cmath&gt;, and &lt;cstdlib&gt;. </strong>You may NOT use <strong>&lt;string&gt;</strong>. You should only use <strong>namespace std</strong>.</li>

 <li>You must use a variety of functions (at least 5) including passing parameters to those functions and returning information from those functions. At least one time, an array (of any size) must be passed to a function (although you may do this more than once).</li>

 <li>All user input must be validated. For example, if a menu allows for 1, 2, or 3 to be entered and the user enters a 4, it will re-prompt the user. However, the user is expected to always enter the correct data type. i.e. If the user is asked to enter an integer, they will. If they are asked to enter a character, they will. You do not need to worry about checking for correct data types.</li>

 <li>You must use at least one multi-dimensional array in this project.</li>

 <li>When the game is initially started, it should prompt the user if they want to load the “default” puzzle or a puzzle from a file. The default puzzle which can be used for initial testing should look like this:</li>

</ul>

<strong>Figure 3. Default Puzzle</strong>

<ul>

 <li>Input files start in row 0 and iterate through the columns then move to row 1 and iterate through the columns all the way to row 4. Each line will have data for exactly one cell. There are three test puzzle files (all are solvable) named <strong>txt</strong>, <strong>proj1_test2.txt</strong>, and <strong>proj1_test3.txt</strong>. We may use different test files and the name of the file should not appear in your code at all.</li>

</ul>

<strong>Figure 4. Load Order from File</strong>

<ul>

 <li>On a player’s turn, the player enters a row and column number. The row and column must start at 1 (unlike the values in the array itself).</li>

 <li>The board will show each of the integers (1-15) or a 0 (representing the blank).</li>

 <li>A tile may only slide into a blank. If a tile is attempted to be slid into a space that already has a value, it will not move there. Additionally, if the tile would leave the board, it will not move either. In both cases, the user should be notified of the illegal move.</li>

 <li>After each slide, the game should check to see if all 15 tiles are in order and the blank is in the bottom right hand corner. If the win condition is met, the game should indicate that the game was won and to re-prompt the user to play again.</li>

 <li>A solved board looks like this:</li>

</ul>

<strong>Figure 5. Solved 15 Puzzle</strong>




<ul>

 <li>Exit and include a thank you message for the user.</li>

 <li>Specific coding requirements include:

  <ul>

   <li>Must use at least 5 different functions.</li>

   <li>Must be able to read a puzzle in the form of a file</li>

   <li>Must use at least one multidimensional array</li>

   <li>Must pass at least one array to a function</li>

   <li>Must not use any global variables (constants are good!)</li>

   <li>Must use at least one switch statement.</li>

   <li>Must use input validation (assume the data is the correct type).</li>

   <li>Must use at least one do..while loop.</li>

   <li>Must use constants as needed.</li>

  </ul></li>

</ul>

<h1>5.   Recommendations</h1>

You are free to implement this with your own functions. While not required, these are some functions that you may want to include:

<ul>

 <li>Start the Game – Sets up the board based on a file or makes the default scenario (with just two out of order for initial testing).</li>

 <li>Select Tile – user chooses the row and column of the tile to slide into the blank.</li>

 <li>Swap Tile – swaps the value of the chosen tile and the blank</li>

 <li>Check Direction – After the user chooses a tile, checks to see if any of the adjacent tiles are empty. If so, swaps them.</li>

 <li>Print the Board – used to display the entire board formatted with the row and columns visible.</li>

</ul>

<h1>6.   Sample Input and Output</h1>

For this project, there are three sample files: <strong>proj1_test1.txt</strong>, <strong>proj1_test2.txt</strong>, and <strong>proj1_test3.txt</strong> and they can be copied from my directory to yours.

First navigate to your project 1 directory. Then run this command:

<strong>cp /afs/umbc.edu/users/j/d/jdixon/pub/cs202/proj1/* .</strong>

Note: the line above goes asterisk, space, then period. This should copy all three files into your working directory.

In the sample output below, user input is colored blue for clarity. After compiling and running proj1, here is a sample run using the default board. As you can see, it can be solved with just one move (there is an example of what happens when you choose the blank itself).




<table>

 <tbody>

  <tr>

   <td width="624">Welcome to the Fifteen GameWould you like to load a board?1. Yes2. No2Loading default1     2     3     41|   1|    2|    3|    4|2|   5|    6|    7|    8|3|   9|   10|   11|   12|4|  13|   14|    0|   15|What is the row (left) and column (top) to slide?43You chose the blankThat tile cannot slide1     2     3     41|   1|    2|    3|    4|2|   5|    6|    7|    8|3|   9|   10|   11|   12|4|  13|   14|    0|   15|No winnerWhat is the row (left) and column (top) to slide?44The tile slid left1     2     3     41|   1|    2|    3|    4|2|   5|    6|    7|    8|3|   9|   10|   11|   12|4|  13|   14|   15|    0|Congrats you’ve won!Play again? (y/n)nThank you for playing the game of fifteen!</td>

  </tr>

 </tbody>

</table>

Here is the <strong>proj1_test2.txt</strong> run.

<table>

 <tbody>

  <tr>

   <td width="624">Welcome to the Fifteen GameWould you like to load a board?1. Yes2. No1What is the file name?proj1_test2.txt1     2     3     41|   0|    2|    3|    4|2|   1|    6|    7|    8|3|   5|   10|   11|   12|4|   9|   13|   14|   15|What is the row (left) and column (top) to slide?21The tile slid up1     2     3     41|   1|    2|    3|    4|2|   0|    6|    7|    8|3|   5|   10|   11|   12|4|   9|   13|   14|   15|No winnerWhat is the row (left) and column (top) to slide?31The tile slid up1     2     3     41|   1|    2|    3|    4|2|   5|    6|    7|    8|3|   0|   10|   11|   12|4|   9|   13|   14|   15|No winnerWhat is the row (left) and column (top) to slide?41The tile slid up1     2     3     41|   1|    2|    3|    4|2|   5|    6|    7|    8|3|   9|   10|   11|   12|4|   0|   13|   14|   15|No winnerWhat is the row (left) and column (top) to slide?42The tile slid left1     2     3     41|   1|    2|    3|    4|2|   5|    6|    7|    8|3|   9|   10|   11|   12|4|  13|    0|   14|   15|No winnerWhat is the row (left) and column (top) to slide?43The tile slid left1     2     3     41|   1|    2|    3|    4|2|   5|    6|    7|    8|3|   9|   10|   11|   12|4|  13|   14|    0|   15|No winnerWhat is the row (left) and column (top) to slide?44The tile slid left1     2     3     41|   1|    2|    3|    4|2|   5|    6|    7|    8|3|   9|   10|   11|   12|4|  13|   14|   15|    0|Congrats you’ve won!Play again? (y/n)nThank you for playing the game of fifteen!</td>

  </tr>

 </tbody>

</table>

Here is an example validating row/column entries. It re-prompts until the user enters a valid value.

<table width="642">

 <tbody>

  <tr>

   <td width="642">Welcome to the Fifteen GameWould you like to load a board?1. Yes2. No2Loading default1     2     3     41|   1|    2|    3|    4|2|   5|    6|    7|    8|3|   9|   10|   11|   12|4|  13|   14|    0|   15|What is the row (left) and column (top) to slide?00What is the row (left) and column (top) to slide?55What is the row (left) and column (top) to slide?44Row: 3 Column: 3The tile slid left1     2     3     41|   1|    2|    3|    4|2|   5|    6|    7|    8|3|   9|   10|   11|   12|4|  13|   14|   15|    0|Congrats you’ve won!Play again? (y/n)</td>

  </tr>

 </tbody>

</table>

<h1>7.   Compiling and Running</h1>

To compile your program, enter the following command at the Linux prompt:

g++ -Wall proj1.cpp -o proj1 (use this command to show warnings – which should be eliminated before turning your code in)

This command runs the GNU C++ compiler (<strong>g++</strong>). The option <strong>-Wall</strong> instructs the compiler to be verbose in its production of warning messages; the option <strong>-o proj1</strong> (hyphen followed by the letter “o”, not the digit zero), instructs the compiler to give the executable program the name <strong>proj1</strong>. If the program compiles correctly, the executable file <strong>proj1</strong> will be created in the current directory.  Your project files should have no warnings or errors when turned in.

At the Linux prompt, enter the command <strong>./proj1</strong> to run your program. It should look like the sample output provided above.

<h1>8.   Completing your Project</h1>

When you have completed your project, you can copy it into the submission folder. You can copy your files into the submission folder as many times as you like (before the due date). We will only grade what is in your submission folder.

Test your code! Make sure that every scenario works. Slide your tiles into each of the corners and make sure they work. Solve a couple of different puzzles.

For this project, you should submit these files to the <strong>proj1</strong> subdirectory:

<strong>proj1.cpp</strong> — should include your implementations of the required functions.

Submitting your project has two steps:

<ol>

 <li>Set up a symbolic link in your home directory to your submission folder. Execute these commands:

  <ol>

   <li><strong>cd ~</strong></li>

   <li>For the next command, copy it exactly – you should not need to modify it at all (<strong>$USER</strong> will automatically populate your user name on GL). Also, notice the space after <strong>$USER</strong> and before <strong>~/cs202proj</strong>.</li>

  </ol></li>

</ol>

<strong>ln -s /afs/umbc.edu/users/j/d/jdixon/pub/cmsc202/$USER ~/cs202proj</strong>

<ol>

 <li>To check that the symbolic link was built successfully, you can type:

  <ol>

   <li><strong>ls ~/cs202proj </strong></li>

   <li><strong>It should list proj1, proj1-late1, proj1-late2 through proj5-late2</strong></li>

  </ol></li>

</ol>




<ol start="2">

 <li>Copy the project files into your proj1 folder. Execute these commands:

  <ol>

   <li>cd to your project 1 folder. An example might be:</li>

  </ol></li>

</ol>

<strong>cd ~/202/projects/proj1</strong>

<ol>

 <li><strong>cp proj1.cpp ~/cs202proj/proj1</strong></li>

</ol>

You can check to make sure that your files were successfully copied over to the submission directory by entering the command

ls ~/cs202proj/proj1

You can check that your program compiles and runs in the <strong>proj1 </strong>directory, but please clean up any <strong>.o </strong>and executable files. Again, do not develop your code in this directory and you should not have the only copy of your program here.







<strong><u>IMPORTANT:</u></strong> If you want to submit the project late (after the due date), you will need to copy your files to the appropriate late folder. If you can no longer copy the files into the proj1 folder, it is because the due date has passed. You should be able to see your proj1 files but you can no longer edit or copy the files in to your proj1 folder. (They will be read only)

<ul>

 <li>If it is 0-24 hours late, copy your files to <strong>~/cs202proj/proj1-late1</strong></li>

 <li>If it is 24-48 hours late, copy your files to <strong>~/cs202proj/proj1-late2</strong></li>

 <li>If it is after 48 hours late, it is too late to be submitted.</li>

</ul>