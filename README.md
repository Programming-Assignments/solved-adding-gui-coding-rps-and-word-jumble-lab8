Download Link: https://assignmentchef.com/product/solved-adding-gui-coding-rps-and-word-jumble-lab8
<br>
In this lab we will be combining our efforts in <strong>top-down programming</strong>, where we deliberately organize and structure our code with main functions and sub functions, but will also add in our skills in Graphic User Interface (<strong>GUI</strong>). We continue to build <strong>abstraction</strong> – where a few small, simple and concrete tasks are packaged together to perform a more general task. The top-down approach helps us organize our code like an <strong>outline</strong> organizes our writing. Again, we start with an algorithm (chart), then translate it into <strong>pseudocode</strong> of comments and function name definitions.




In the last lab you created code to play Rock-Paper-Scissors. You will be working with the same code (modify to resolve comments from your last lab), but rather than using input() you will now collect input using the GUI. Be creative about displaying messages to the player.




<h3>Submittal to Turnitin.com</h3>

Because plagiarism in coding is dishonest, unethical, and is against the Miramonte Honesty Policy, you are required to submit your code to Turnitin.com.  Make a Google Doc with your final code for Rock-Paper-Scissors and Word Jumble, and submit it to<u><a href="https://www.turnitin.com/"> turnitin.com</a></u>, Lab #8.







<h2>Problem #1 – Rock-Paper-Scissors Reprise (with GUI)</h2>

Game Requirements

<ol>

 <li>Display messages on the canvas that explain to the user how to choose Rock, Scissors, or Paper. They may not input their choice with any text input box.</li>

 <li>Once the player makes their selection, have the computer make a selection. Display both the player’s and computer’s selection on the Canvas (it is good programming practice to also display on the console to help you debug).</li>

 <li>Display the outcome (“You win!” or “Computer wins!”)</li>

 <li>Tally and update the score after each iteration of the game.</li>

 <li>You do not have to ask the user to play again… you can assume they will, but do give them some method to Quit when they are ready.</li>

 <li>When they quit, display a parting message and the final score.</li>

</ol>




<h3>RPS starter code</h3>

<table width="0">

 <tbody>

  <tr>

   <td width="726"><u><a href="https://py3.codeskulptor.org/#user303_BkZlCk7i6wnA7XC.py">Rock-Paper-Scissors GUI starter code</a></u> – copy/paste into Codeskulptor and build code.</td>

  </tr>

  <tr>

   <td width="726">import simpleguiimport random“””Overview of Game Logic:1.  Screen is drawn with blank values, input method for player RPSis explained/presented2.  Player selects R, P, or S using some form ofGUI input (no input box).3.  Computer randomly selects option R, P or S4.  Winner is identified, results shared, score updated and posted5.  Repeats #2-4 each time a button, key-stroke, or mouse-clickis initiated.4.  Stops when quit is pressed/clicked.“””###### INITIALIZATION CODE ###################Global variables, changed within functions below# Canvas Dimensionscanvas_width =canvas_height =####### RPS algorithm helper functions #########Computer Generatordef comp_choice():pass“””Will randomly select Rock, Paper, or Scissors. “””#global variables here.#pick a random R, P, or S….#Update computer choice message for draw handler#call winner() to determine outcome#Determine Winnerdef winner():pass“””Determine the winner then updates the score”””#global variables here#determines the winner#updates the necessary draw(canvas) variables to show messages########### EVENT HANDLERS ######################define event handlers for mouse click, buttons, input box, key_strokes, draw# Player Choice Selection (not input box).def button_quit_handler():pass#global variable here#updates the necessary draw(canvas) variables# Handler to draw on canvasdef draw(canvas):pass#Player choice: use canvas.draw_text(parameters), pass in message as variable#Computer choice#Winner text and score update#Any additional messaging# Create a frame and assign callbacks to event handlersframe = simplegui.create_frame(“Rock, Paper, Scissors”, canvas_width, canvas_height)frame.add_label(‘Player Choice:  Select One’)frame.add_button(#add parameters)frame.set_draw_handler(#add parameter)#add more frame.set for key handler, buttons, mouse click, etc.# Start the frame animationframe.start()</td>

  </tr>

 </tbody>

</table>




<table width="0">

 <tbody>

  <tr>

   <td width="726">Insert Final, working Rock-Paper-Scissors with GUI code – include detailed comments</td>

  </tr>

  <tr>

   <td width="726">&lt;&lt;your code here&gt;&gt; – please format with Code Blocks add-on – Python, github-gist    </td>

  </tr>

 </tbody>

</table>




<strong> </strong>

<h2>Problem 2: Word Jumble</h2>

As you solve a problem or write a computer program, the process should be:

<ol>

 <li>Understand the task/purpose of code</li>

 <li>Organize main task into sub-tasks and consider task flow (sequencing)

  <ol>

   <li>Create flow structure with an algorithm flow chart (whiteboard!). Consider collaborating with a programming partner as you plan.</li>

   <li>Create pseudocode outline with comments, naming key flow functions.</li>

  </ol></li>

 <li>Build, code and test sub-functions first. Debug as you go. Revise plan/structure as necessary.</li>

 <li>Combine sub-functions into larger program and test, test, test! Revise plan as necessary.</li>

 <li>Consider extensions or improvements to original design.</li>

</ol>

Keep your words to 5 and 6 letters each.  This is like the Jumble in the newspaper and online games and will make the GUI display easier and more aesthetically pleasing.

<u><a href="#_pkxs5h7pby6s">Overview</a></u>

<u><a href="#_sp6rwcl86zbz">Submission:</a></u>

<u><a href="#_wbfaenhkczfp">Development Process</a></u>

<u><a href="#_b52ujz830rmn">Part 1:  Backend Development</a></u>

<u><a href="#_cynkcszdmm3b">Part 2: Frontend Development</a></u>







<h3>Overview</h3>

You need to create a program that allows a user to guess a word that has been jumbled together. This project focuses on Strings and String manipulation, as well as presenting output with the GUI.

<h3>Submission:</h3>

Note, this is modeled after the Create Performance Task that you will submit as part of your <u><a href="https://apcentral.collegeboard.org/courses/ap-computer-science-principles/exam">AP Portfolio</a></u>.  You will submit your code write up via Google Classroom and <u><a href="http://turnitin.com/">TurnItIn.com</a></u>

<h3>Support Materials:</h3>

<ol>

 <li><u><a href="https://www.youtube.com/watch?v=3CpPQY1BkAI&amp;feature=youtu.be">Video of Frontend and Backend</a></u></li>

 <li><u><a href="https://py3.codeskulptor.org/#user303_mPw8UhfyMUaN3b0.py">String randomizer</a></u></li>

</ol>

<h3>Development Process</h3>

<h4>Part 1: Backend Development</h4>

You will create a word jumble game. You should use functions to help you both pick a word from a list, scramble it and then prompt the user for guesses. Below is a rough outline of the pseudocode. You do NOT need to use this structure, but you SHOULD have some structure in place before you start writing code. Think of this as the outline.




Your first working version of the game will rely on input() and printing to the Console. We call this “Backend Development,” where we get the algorithm and flow working correctly.




Note, you may find the method, random.shuffle(some_list), to be helpful when scrambling the word. You will find the documentation in the <u><a href="https://py3.codeskulptor.org/docs.html#random-shuffle">Random Module</a></u>




<strong>Optional Extension</strong>

Add a timer to your game. Give the user 30 seconds to guess the jumbled word.




The user is entering their guess in an input box.






















<table width="0">

 <tbody>

  <tr>

   <td width="726"><strong>Insert Word Jumble without GUI </strong><strong>Algorithm (photo from whiteboard is fine, or use Google Draw algorithm)</strong></td>

  </tr>

  <tr>

   <td width="726">  </td>

  </tr>

  <tr>

   <td width="726"><strong>Insert Word Jumble without GUI</strong><strong> Pseudocode here (outline of comments and function definitions that demonstrate intended flow)</strong></td>

  </tr>

  <tr>

   <td width="726">import randomword_list = []word = “”scram_list = []scrambled_word = “”users_guess = “”def make_word_list(): #makes list of wordsdef choose_word(): #random word from listdef scramble_letters_in_word(): #shuffles letters of random word from listdef display_scrambled_word(): #displays shuffled worddef user_guess(text_input): #user inputdef check_if_correct(): #checks if correct/matches unshuffled word; if it does not match, asks againdef play_jumble(): #starts jumble, asks if user wants to playdef play_again(): #asks user to play againplay_jumble()</td>

  </tr>

  <tr>

   <td width="726"><strong>Insert Final, working Word Jumble without GUI code – include detailed comments</strong></td>

  </tr>

  <tr>

   <td width="726">import randomword_list = []word = “”scram_list = []scrambled_word = “”users_guess = “”guesses= 0def make_word_list():global word_listword_list = [“apple”, “gamer”, “chair”, “happy”]def choose_word():global wordword = “”word = random.choice(word_list)def scramble_letters_in_word():global scram_listscram_list = []scram_list.extend(word)random.shuffle(scram_list)def display_scrambled_word():global scrambled_wordscrambled_word = “”for letter in scram_list:scrambled_word = scrambled_word + letterprint (scrambled_word)def user_guess(text_input):global users_guessusers_guess = text_inputcheck_if_correct()def check_if_correct():global guessesif word == users_guess:guesses +=1print (“You got it!”)print (“Guesses: “, guesses)print (“”)play_again()else:guesses +=1print (“You did not get it!”)print (“Guesses: “, guesses)user_guess(input(“Try again, unjumble the word!”))def play_jumble():play_game = input(“Do you want to play jumble?”)if play_game[0].upper() == “Y”:make_word_list()choose_word()scramble_letters_in_word()display_scrambled_word()user_guess(input(“Unjumble the word!”))elif play_game[0].upper() == “N”:print (“Thanks for playing.”)else:play_jumble()def play_again():global guessesjumble_again = input(“Do you want to play again?”)if jumble_again[0].upper() == “Y”:guesses = 0make_word_list()choose_word()scramble_letters_in_word()display_scrambled_word()user_guess(input(“Unjumble the word!”))elif jumble_again[0].upper() == “N”:print (“Thanks for playing.”)play_jumble()</td>

  </tr>

 </tbody>

</table>




<h4>Part 2: Frontend Development</h4>

Once you have a working game using the input() and console, you will now modify it to include GUI.




You will create a GUI (similar to the one below). You should be able to use the majority of your code from part 1 for the underlying logic, however you may need some new variables and a draw handler to make the GUI display correctly. Remember all your print statements must be turned into variables that can be displayed on the canvas.







Here is <u><a href="https://py3.codeskulptor.org/#user303_1vJRtW91MTDOxGe.py">some suggested code </a></u>to include in your GUI version of the game.

<table width="0">

 <tbody>

  <tr>

   <td width="726"># template for jumble with GUIimport simpleguiimport random###### INITIALIZATION CODE ################### global variables some of these variables will initially be empty strings# since they will not be displayed at the start of the game.####### JUMBLE algorithm helper functions ######### insert working algorithm code from your Backend design###### MAIN PROGRAM CALLED WHEN START BUTTON CLICKED ####def gameison():# global variables# reset the global variables at the start of each round – new scrambled word.pass########### EVENT HANDLERS ######################define event handlers for mouse click, buttons, input box, key_strokes, drawdef text_input():# global variables# this code will be similar to your userguess() function code in non-GUI# jumble but the print statements will have to used to create global variables# that are displayed on the canvas.def button_start_handler():# global variablesgameison()def button_exit_handler():# global variablesframe.stop()def draw(canvas):# remember this function is called 60 times a second.frame = simplegui.create_frame(‘Jumble’, 700, 500)frame.add_button(# add parameters for a start to play button)frame.add_button (# add parameters for an end to play button)frame.add_input(# add parameters for an input pox)frame.set_draw_handler(# add parameter)frame.start()</td>

  </tr>

 </tbody>

</table>




<table width="0">

 <tbody>

  <tr>

   <td width="726"><strong>Insert Word Jumble with GUI</strong><strong> Pseudocode here (outline of comments and function definitions that demonstrate intended flow – use the starter code but insert your functions to run the backend Jumble Algorithm)</strong></td>

  </tr>

  <tr>

   <td width="726">&lt;&lt;pseudocode here&gt;&gt;     </td>

  </tr>

  <tr>

   <td width="726"><strong>Insert Final, working Word Jumble with GUI code – include detailed comments</strong></td>

  </tr>

  <tr>

   <td width="726">&lt;&lt;code here&gt;&gt; – please format with Code Blocks add-on – Python, github-gist     </td>

  </tr>

 </tbody>

</table>








