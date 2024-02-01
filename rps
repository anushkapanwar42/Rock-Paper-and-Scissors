#include <conio.h>
#include <stdio.h>
#include <stdlib.h>
#include <time.h>
char mach_input(){
    //generation of machine input helds here.
     srand(time(NULL));
     char char_set[] = {'S', 'R', 'P'};
     int set_size = sizeof(char_set) / sizeof(char);
     int random_index = rand() % set_size;
     char random_char = char_set[random_index];
     return random_char;

}
void win(char user){
    char machine = mach_input();
    printf(" %c\n",machine);
    // winnings conditions are defined here
    if(machine==user){
        printf("Result: Draw");
    }
    else if((machine=='R'&& user=='P')||(machine=='S'&& user=='R')||(machine=='P'&& user=='S')){
        printf("Result: You won.");
    }
    else if((machine=='P'&& user=='R')||(machine=='R'&& user=='S')||(machine=='S'&& user=='P')){
        printf("Result: Machine Won.");
    } 
}
void main()
{
    printf("*********************************************************************\n");
    printf("Welcome to the Game: Rock, Paper and Scissors.\n");
    char input;
    int c;
    do{
    printf("Enter a character: \n('S' stands for 'Scissors')\n('P' stands for 'Paper')\n('R' stands for 'Rock')\n ");
    char user;
    scanf(" %c",&user);
    win(user);
    printf("\nWould you like to play the game again?(Y/N): ");
    while ((input = getchar()) != '\n' && input != EOF); //this line clears the input buffer
    scanf("%c",&input);
    printf("*********************************************************************\n");
    }
    while(input=='Y');
  
}
