# solved-comp-2401-assignment-5
**TO GET THIS SOLUTION VISIT:** [SOLVED:COMP 2401 — Assignment #5](https://www.ankitcodinghub.com/product/solvedcomp-2401-assignment-5/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;1381&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;5&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (5 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;SOLVED:COMP 2401 -- Assignment #5&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (5 votes)    </div>
    </div>
You will write a program in C, in the Ubuntu Linux environment, to simulate a two-player game of Twenty Questions, as a distributed system over the School of Computer Science network. One player (the oracle) chooses an object that the other player (the guesser) tries to guess by asking the oracle one question at a time. At every turn, the guesser asks a yes/no question, or tries to guess the object. The oracle responds by signalling one of three responses: yes, no, or win. If the guesser correctly guesses the object within 20 questions, s/he wins, otherwise the oracle wins. The winning player is given a choice of quitting the game, or playing another round. If s/he opts to play again, s/he becomes the oracle for the next round.In this assignment, you will:• implement a game between two users on different computers, communicating over TCP/IP sockets• modify client-server code so that a single executable program can switch between client mode and server modeInstructions1. Process startupYou are writing code for a single executable program. Both guesser and oracle players will be running their own copy of the same program, but executing on different computers that are networked together.Your program initiates a connection to another game process as follows:• the user may specify an IP address on the command line or not• if an IP address is specified, then the game process initiates a connection using TCP/IP sockets to the other game process running at the specified IP address• if no IP address is specified, then the game process waits for another game process to initiate a connection2. Game logicThe Twenty Questions game logic works as follows:• setting up a roundo the player on the game process that initiated the connection takes on the role of guessero the other player becomes the oracle• during the roundo at each turn, the guesser is prompted for a yes/no question (questions should be numbered)o the question is sent to the oracle’s game processo the oracle user enters a response using signals; do not prompt the oracle for input! the SIGINT (Ctrl-C) signal indicates a yes answer to the question the SIGTSTP (Ctrl-Z) signal indicates a no answer to the question the SIGQUIT (Ctrl-\) signal is a win answer, meaning that the guesser has correctly guessed the objecto both players see all the questions asked so far, along with the answero if the guesser correctly guesses the object, s/he winso if the number of questions reaches 20 without a correct guess, the oracle wins• ending a roundo when a player wins, s/he is prompted to either play another round or quito the losing player does not get a choice and must play again if the winner chooses to do soo if the winner decides to play again, s/he becomes the oracle, and a new round starts upo if the winner decides to quit: the winner’s game process closes the connection, cleans up all its resources, and terminates the loser’s game process waits for a new connection to be initiatedCOMP 2401 — Assignment #5 Fall 2013 2/2Constraints• Design:o you must separate your code into modular, reusable functionso never use global variables, unless otherwise instructed• Implementation:o your program must perform all basic error checking and clean up resources upon terminationo it must be thoroughly commented• Executiono programs that do not compile, do not execute, or violate any constraint are subject to severe deductionsSubmissionYou will submit in cuLearn, before the due date and time, one tar file that includes all the following:• all source and header files• a Makefile• a readme file, which must include:o a preamble (program author(s), purpose, list of source/header/data files)o exact compilation command(s)o launching and operating instructionsGrading• Marking breakdown:ComponentMarksprocess startup40game logic60• Assignment grade: Your grade will be computed based on the completeness of your implementation, plus bonus marks, minus deductions.• Deductions: 100 marks if:o any files are missing from your submission, or if they are corrupt or in the wrong format 50 marks if:o the Makefile is missingo the code does not compile using gcc in the Ubuntu Linux shell environmento code cannot be tested because it doesn’t run 25 marks if:o your submission consists of anything other than exactly one tar fileo your program is not broken down into multiple reusable, modular functionso your code is not correctly separated into header and source fileso your program uses global variables (unless otherwise explicitly permitted)o the readme file is missing or incomplete 10 marks for missing comments or other bad style (non-standard indentation, improper identifier names, etc)• Bonus marks: Up to 5 extra marks are available for fun and creative additional features
