#include <stdio.h>
#include<time.h>
#include<stdlib.h>
int main() {
    // Write C code here
    int number,guess, attempts=1;
    srand(time(0));
    number = rand()%100+1; // number between 1 to 100
     //printf("the number is %d\n", number);
     printf(" best of luck ! \n");
    do{
        printf("enter a number between 1 to 100 :");
        scanf("%d",&guess);
        if(guess>number){
            printf("enter a smaller number please!\n");
        }
        else if(guess<number){
            printf("enter a greater number please!\n");
        }
        else{
            printf("You guessed it correct in %d attempts\n",attempts);
        }
        attempts++;
    }while(number!= guess);
    printf("thank you for playing this game");

    return 0;
}
