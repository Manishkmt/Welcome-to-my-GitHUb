 Welcome-to-my-GitHUb
Here you can enjoy  new project of c/c++
All the project are created by _._manish_._kmt_._

This project of the game like guessung and search random number. you can play this and really enjoy the game.

#include<stdio.h>
#include<stdlib.h>
#include<time.h>

int main()
{
   
  int random, guess;
  int no_of_guess = 0;
  srand(time(NULL));

  printf("Welcome to the World of Guessing Numbers Game\n");
  random = rand()  % 100 - 1; //Generating between 0 to 100
  

  do {
    printf("\nPlease enter your Guess betwwen (1 to 100):");
    scanf("%d",&guess);
    no_of_guess++;

    if(guess < random) {
      printf("\nGuess a larger number:");
    } else if(guess > random) {
      printf("\nGuess a smaller number:");

    } else {
      printf("\nCONGRATULATIONS !! You have successfully guessed the number in %d attempts",no_of_guess);
    }
    

  }while(guess != random);

  printf("\n Bye Bye , Thanks for Playing.");
  printf("\n Developed By : _._manish_._kmt_._");

return 0;
}
