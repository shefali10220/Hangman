# Hangman
A normal hangman game ,where the user can guess letters before they kill the innocent man.

The Main file doesnt gove any hint to the user,the user has to guess the word without a hint.
Meanwhile the w_hint_main file gives the user a hint ,which makes it easier to guess the word 

In this game we first start by creating a word list with many random words. after this list is made we go to our main class and select one word using the random library to select the word for us(lets call this the game word). After this is done , the word is converted to upper case. The lenght of the word is taken using the len() function. After this "_" characters times the lenght of the word is displayed on the screen for the user to guess the word. 
Before the user starts guessing, guessed flag is set to zero , a guesses list is emptied and the tries is set to 6 as the user has 6 tries to start guessing the word.The program checks if the word guessed is actually a letter or not and it checks if its there in the guessed list first, then it checks whether the guessed letter is  present in the game word using the "in" keyword.

Case Senario 1: The guessed letter is present in the game word.

              The guessed letter replaced the "_". to do this a for look is used. Here the for loop traverses through the game word and find the indice of the letter and then using this number the letter is changed using join.
              
Case Senario 2: The guessed letter isnt present in the game word.

                Sub case a: the letter is present in the guessed list.
                            If the guessed letter is already there in the list, an alert is thrown and and the number of tries isnt decreased.
                            
                Sub case b : The letter isnt ever guessed
                             If the letter isnt present in the guessed listed, this word is appended to the list along with the number of tries decreasing.
                          
Case Senario 3: The number of tries are over:

                After the tries flag reaches zero , the game ends and the user is displayed the word and qasked whether they wanna play again, If yes they can press Y                 else a N.
                             
