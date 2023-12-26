#include <stdio.h>
#include<conio.h>
#include <stdlib.h>
void main(){
srand(time(0));
/*
Rock Paper Scissor is one of the most common games played by everyone once in his childhood, where two persons use their hands and chooses random objects between rock, paper, or scissor,
and their choice decides the winner between them. What if a single person can play this game? With a computer, just by using a single C application,
we can design the game Rock Paper Scissor application
just using basic C knowledge like if-else statements, random value generation, and input-output of values.
Created application has a feature where we can play the game, and maintain the score of Person 1 and Person 2.
*/
//user1
int rps1;
printf("Enter Rock(1) Paper(2) Scissors(3) User 1\n");
scanf("%d",&rps1);
// win factor
// generates a random number between 1 and 3
int compwin=(rand()%3)+1;
if(rps1==1 && compwin==1){
    printf("Draw");
}
else if(rps1==1 && compwin==2){
    printf("Computer wins and your choice:%d and you lose and computer selection is:%d",rps1,compwin);
}
else if(rps1==1 && compwin==3){
    printf("You win and your choice:%d,computer loses and computer selection is:%d",rps1,compwin);
}
else if(rps1==2 && compwin==1){
   printf("You win and your choice:%d,computer loses and computer selection is:%d",rps1,compwin);
}
else if(rps1==2 && compwin==2){
     printf("Draw");
}
else if(rps1==2 && compwin==3){
    printf("Computer wins and your choice:%d and you lose and computer selection is %d",rps1,compwin);
}
else if(rps1==3&& compwin==1){
   printf("Computer wins and you lose and your choice:%d and computer selection is %d",rps1,compwin);
}
else if(rps1==3 && compwin==2){
     printf("You win and your choice:%d,computer loses and computer selection is %d",rps1,compwin);
}
else if(rps1==3 && compwin==3){
   printf("Draw");
}
else{
    printf("Re-enter value");
}
}
