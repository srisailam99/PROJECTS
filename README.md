// CHAT BOT ----> WORKS AS ON CMD COMMANDS

// ai chat bot in c programming
#include<stdio.h>                                 // THE CODE CLASS YOUTUBE CHANNEL
#include<conio.h>
#include<string.h>
#include<time.h>
#include<stdlib.h>

char user_input[100];
int main()
{   system("cls");
    printf("welcome in ai chat bot\n");
    while(1)
    {
     printf("user ==> ");
     gets(user_input);
     if(strcmp(user_input,"exit")==0)
     {
         system("cls");
         printf("bot ==> ok byy\n");
         break;
     }
     else if(strcmp(user_input,"change color")==0)
     {
         system("color a");
     }
     else if(strcmp(user_input,"hi")==0)
     {
         printf("bot ==> hi sir\n");
     }
     else if(strcmp(user_input,"what is your name")==0)
     {
         printf("bot ==> my name is samantha ,sir\n");
     }
     else if(strcmp(user_input,"how are you")==0)
     {
         printf("bot ==> i'm fine, how can i help you? \n");
     }
     else if(strcmp(user_input,"i love you")==0)
     {
         printf("bot ==> love you too darling\n");
     }
     else if(strcmp(user_input,"open chrome")==0)
     {
         printf("ok sir , opeaning chrome browser \n");
         system("start chrome");
     }
     else if(strcmp(user_input,"open notepad")==0)
     {
         printf("ok sir , opeaning notpad editor \n");
         system("start notepad");
     }
     else if(strcmp(user_input,"open cmd")==0)
     {
         printf("ok sir , opeaning cmd terminal \n");
         system("start cmd");
     }
     else if(strcmp(user_input,"time")==0)
     {
         time_t s, val =1 ;
         struct tm* current_time;
         //time in second
         s = time(NULL);
         current_time = localtime(&s);
         //print time in minute
         //print hour and second
         printf("bot ==> %02d:%02d:%02d\n",current_time->tm_hour,current_time->tm_min,current_time->tm_sec);
     }
     else if(strcmp(user_input,"open youtube")==0)
     {
        printf("ok sir , opeaning youtube \n");
        system("start http://youtube.com");
     }
      else if(strcmp(user_input,"open google")==0)
     {
        printf("ok sir , opeaning google \n");
        system("start http://google.com");
     }
    }
    return 0;
}
