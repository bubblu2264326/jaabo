#include<stdio.h>
#include<conio.h>
#include<stdlib.h>
#include<windows.h>
#include<time.h>
#include<string.h>
#include<math.h>
#include<ctype.h>
typedef struct {
   	char name[20];
   	char edu[15];
	char profession[12];
	char available_days[12];
	char contact[20];   //this can either be your e mail or phone no
	int pay_per_hour;
	char work_experince[10];
	int availible_hours;
}employee;
typedef struct{
                          //p_no=professions
	 employee n[100];
}profession;

int main(){

     profession p_no[7];
	int choice,a;
	intro();
	system("cls");
	while(choice!=4){
		box();
	jump(10,6);
    printf("Select  Desire Choice  :  ");
    jump(10,8);
    printf("1 : Are you Customer ?? ");
    jump(10,10);
    printf("2 : Are you Employee ?? ");
    jump(10,12);
    printf("3 : Are you Admin ?? ");
    jump(10,14);
    printf("4 : Exit ");
    jump(10,16);
    scanf("%d",&choice);
    system("cls");
	if(choice==1){
		int r,u;
		box();
    //	printf("1.electrician\n2.cleaner\n3.plumber\n4.mechanic\n5.carpenter\nenter your choice: ");
    jump(10,6);
    printf("Select The labour  : ");
    jump(10,8);
    printf("1 : Electricain ");
    jump(10,10);
    printf("2 : Cleaner ");
    jump(10,12);
    printf("3 : Plumber ");
    jump(10,14);
    printf("4 : Mechanic ");
    jump(10,16);
    printf("5 : Carpenter ");
    jump(10,18);
    	
		scanf("%d",&a);
    	system("cls");
    
	//	printf("Make The choice\n\t\t1.Do You want To Search a employee of Specific rate?\n\n\t\t2.Do You want To Search a employee of Specific shift(i.e Morning,Evening)?\n\n\t\t3.All\n\n\t\t");
	box();
	jump(10,6);
    printf("Enter your Choice : ");
    jump(10,8);
    printf("1 : Enter a employee of Specific rate?");
    jump(10,10);
    printf("2 : Enter  Specific shift(i.e Morning,Evening) ");
    jump(10,12);
    printf("3 : All");
    jump(10,14);
        	scanf("%d",&r);
        	system("cls");
        	switch(r){
        	case 1:
        		    box();
        		    jump(10,12);
        			printf("Enter The Pay_per_Hour  Range: ");
        			jump(10,14);
        			scanf("%d",&u);
        			system("cls");	
         for(int j=0;j<100;j++){
          if(p_no[a].n[j].pay_per_hour<u&&p_no[a].n[j].pay_per_hour>0){
          	        jump(10,6);
		            printf("name:%s\n",p_no[a].n[j].name);
		            jump(10,8);
        			printf("your contact: %s\n",p_no[a].n[j].edu);
        			jump(10,10);
        			printf("pay per hour: %d\n",p_no[a].n[j].pay_per_hour);
        			jump(10,12);
        			printf("work experience: %s\n",p_no[a].n[j].work_experince);
        			jump(10,14);
        			printf("available days: %s\n", p_no[a].n[j].available_days);
        			jump(10,16);
        		//	printf("available hours: %d\n",p_no[a].n[j].availible_hours);
    }
		 }
		  printf("Press any key to continue...");
		 getch();
		 system("cls");
		 break;
        			
        		case 2:
        			box();
        			//printf("Enter The shift which  want enmployee:\n1.Morning(8am-12pm)\n2.Afternoon(1pm-5pm)\n3.Evening(6pm-10pm)\n");
        			jump(10,6);
    printf("Enter The shift in which  want enmployee: : ");
    jump(10,8);
    printf("1 : Morning(8am-12pm)");
    jump(10,10);
    printf("2 : Afternoon(1pm-5pm) ");
    jump(10,12);
    printf("3 : Evening(6pm-10pm)");
    jump(10,14);
        			fflush(stdin);
        			jump(10,16);
        			scanf("%d",&u);
        			system("cls");
        		// 3shifts ka opyion da daina hain
        		switch(u){
        			case 1:
        					 for(int j=0;j<100;j++){
          if(p_no[a].n[j].availible_hours==1&&p_no[a].n[j].availible_hours!=0){
		                     	        jump(10,6);
		            printf("name:%s\n",p_no[a].n[j].name);
		            jump(10,8);
        			printf("your contact: %s\n",p_no[a].n[j].edu);
        			jump(10,10);
        			printf("pay per hour: %d\n",p_no[a].n[j].pay_per_hour);
        			jump(10,12);
        			printf("work experience: %s\n",p_no[a].n[j].work_experince);
        			jump(10,14);
        			printf("available days: %s\n", p_no[a].n[j].available_days);
        			jump(10,16);
        		//	printf("available hours: %d\n",p_no[a].n[j].availible_hours);
    }
		 }
		  printf("Press any key to continue...");
		 getch();
		 system("cls");
		 break;
        			case 2:
        					 for(int j=0;j<100;j++){
          if(p_no[a].n[j].availible_hours==2&&p_no[a].n[j].availible_hours!=0){
		                      	        jump(10,6);
		            printf("name:%s\n",p_no[a].n[j].name);
		            jump(10,8);
        			printf("your contact: %s\n",p_no[a].n[j].edu);
        			jump(10,10);
        			printf("pay per hour: %d\n",p_no[a].n[j].pay_per_hour);
        			jump(10,12);
        			printf("work experience: %s\n",p_no[a].n[j].work_experince);
        			jump(10,14);
        			printf("available days: %s\n", p_no[a].n[j].available_days);
        			jump(10,16);
        		//	printf("available hours: %d\n",p_no[a].n[j].availible_hours);
    }
		 }
		  printf("Press any key to continue...");
		 getch();
		 system("cls");
		 break;
		 	case 3:
        					 for(int j=0;j<100;j++){
          if(p_no[a].n[j].availible_hours==3&&p_no[a].n[j].availible_hours!=0){
		                      	        jump(10,6);
		            printf("name:%s\n",p_no[a].n[j].name);
		            jump(10,8);
        			printf("your contact: %s\n",p_no[a].n[j].edu);
        			jump(10,10);
        			printf("pay per hour: %d\n",p_no[a].n[j].pay_per_hour);
        			jump(10,12);
        			printf("work experience: %s\n",p_no[a].n[j].work_experince);
        			jump(10,14);
        			printf("available days: %s\n", p_no[a].n[j].available_days);
        			jump(10,16);
        			//printf("available hours: %d\n",p_no[a].n[j].availible_hours);
    }
		 } 
		 
		 getch();
		 system("cls");
		 break;
						
				}
        		 
		 case 3:
		 	 for(int j=0;j<100;j++){
          if(p_no[a].n[j].pay_per_hour!=0){
		             jump(10,6);
		            printf("name:%s\n",p_no[a].n[j].name);
		            jump(10,8);
        			printf("your contact: %s\n",p_no[a].n[j].edu);
        			jump(10,10);
        			printf("pay per hour: %d\n",p_no[a].n[j].pay_per_hour);
        			jump(10,12);
        			printf("work experience: %s\n",p_no[a].n[j].work_experince);
        			jump(10,14);
        			printf("available days: %s\n", p_no[a].n[j].available_days);
        			jump(10,16);
        			//printf("available hours: %d\n",p_no[a].n[j].availible_hours);
    
		 }
        		
			}
			printf("Press any key to continue...");
		 getch();
		 system("cls");
			break;
		
    }
	}
        
				
	
	
	else  if(choice==2){
		int i=0,ch1;
		
	  printf("\t\t\t#### FORM OF EMPLOY #####\n");
	 // printf(" Your Profession name:\n1.electrician\n2.cleaner\n3.plumber\n4.mechanic\n5.carpenter\nenter your choice: ");
	 	box();
    //	printf("1.electrician\n2.cleaner\n3.plumber\n4.mechanic\n5.carpenter\nenter your choice: ");
    jump(10,6);
    printf("Select The Profession  : ");
    jump(10,8);
    printf("1 : Electricain ");
    jump(10,10);
    printf("2 : Cleaner ");
    jump(10,12);
    printf("3 : Plumber ");
    jump(10,14);
    printf("4 : Mechanic ");
    jump(10,16);
    printf("5 : Carpenter ");
    jump(10,18);
    	
	  scanf("%d",&ch1);
	  fflush(stdin);
	  system("cls");
	  //printf("%s\n",n[i].profession);
	  	box();
	  	jump(10,6);
	  printf("Enter Your Name: ");
	  fflush(stdin);
	  jump(10,8);	  
	  gets(p_no[ch1].n[i].name);
	  fflush(stdin);
	  jump(10,10);
	  printf("enter your education: ");
	  jump(10,12);
	  gets(p_no[ch1].n[i].edu);
	  fflush(stdin);
	jump(10,14);
	  printf("available days: ");
	  jump(10,16);
	  fflush(stdin);
	  gets(p_no[ch1].n[i].available_days); 
	  fflush(stdin);
	  system("cls");
	 // printf("Enter The shift :\n1.Morning(8am-12pm)\n2.Afternoon(1pm-5pm)\n3.Evening(6pm-10pm)\n ");
	 box();
	 jump(10,6);
    printf("Enter The shift in which  want To Work: : ");
    jump(10,8);
    printf("1 : Morning(8am-12pm)");
    jump(10,10);
    printf("2 : Afternoon(1pm-5pm) ");
    jump(10,12);
    printf("3 : Evening(6pm-10pm)");
    jump(10,14);
	  scanf("%d",&p_no[ch1].n[i].availible_hours);
	  jump(10,16);
	  //gets(p_no[ch1].n[i].availible_hours);
	  system("cls");
	  fflush(stdin);
	  box();
	 jump(10,6);
	  printf("Enter Your contact:");
	  jump(10,8);
	  fflush(stdin);
	  gets(p_no[ch1].n[i].contact);
	  jump(10,10);
	  fflush(stdin);
	  printf("Enter Your Pay Per Hour: ");
	  jump(10,12);
	  scanf("%d",&p_no[ch1].n[i].pay_per_hour);
	  fflush(stdin);
	  jump(10,14);
	  printf("Enter Your Experince: ");
	  jump(10,16);
	  gets(p_no[ch1].n[i].work_experince); 
	   jump(10,18);
	   printf("Press any key to continue...");
		 getch();
		 system("cls");s
	  i++;
	}
	else if(choice==3){             //admin portal to maintai the data of employee.
		int c;                      //we gave admin to read write acess by using filing
	while(1){
		printf("Welcome To admin Portal\nEnter The password\n To exit Press 0:");
		scanf("%d",&c);
		if(c==123){
		 for(int j=0;j<100;j++){
          
		            printf("name:%s\n",p_no[a].n[j].name);
        			printf("your contact: %s\n",p_no[a].n[j].edu);
        			printf("pay per hour: %d\n",p_no[a].n[j].pay_per_hour);
        			printf("work experience: %s\n",p_no[a].n[j].work_experince);
        			printf("available days: %s\n", p_no[a].n[j].available_days);
        			printf("available hours: %d\n",p_no[a].n[j].availible_hours);
    
		 }
		
		}
		else if(c==0){
			break;
		}
		else{
			printf("Wrong password");
		}
		}
	}
	else{
		//printf("Wrong choice");
		break;
	}

}
}
void jump(int x,int y)
{
        COORD c;
        c.X=x;
        c.Y=y;
        SetConsoleCursorPosition(GetStdHandle(STD_OUTPUT_HANDLE),c);
}
void box()
{
	int i;
	
/*	for ( i=17 ; i<=54 ; i++ ) // upper border
	{
		jump(i,4);
		printf("%c",176);
	}*/
	for ( i=2 ; i<=30 ; i++ ) // for y left
	{
		jump(4,i);
		printf("*");
	}
	for ( i=4 ; i<=70 ; i++ ) // for x up
	{
		jump(i,2);
		printf("*");
	}
	for ( i=4 ; i<=70 ; i++ ) // for x down
    {
		jump(i,30);
		printf("*");
	}
	for ( i=2 ; i<=30 ; i++ ) // for y right
	{
		jump(70,i);
		printf("*");
	}
}
int intro()
{
    box();
	int i,j;
	for ( i=17 ; i<=54 ; i++ ) // upper border
	{
		jump(i,4);
		printf("%c",176);
	}
 
    printf("\n\t\t\t   <---:J A A B O:--->");  
	 for ( i=17 ; i<=54 ; i++ ) // lower border
	{
		jump(i,6);
		printf("%c",176);
	}
	jump(26,8);
    printf("W  E  L  C  O  M  E");
    jump(29,11);
    printf("Developed By:");
    jump(24,13);
    printf("MUHAMMAD ABDUL REHMAN 22K-4291");
    jump(24,14);
    printf("JUNAID ASIF 22K-4169");
    jump(24,15);
    
    jump(24,16);
    
    jump(26,19);
    printf("Course  Instructor:");
    jump(28,21);
    printf("Ms Ayesha Ali");
    jump(15,23);
    printf("LOADING...");
     for ( i=15 ; i<=55 ; i++ ) // loader;
	{
		jump(i,24);
		printf("%c",178);
	}
	jump(22,28);
    printf("Press any key to continue...");
    getch();
    
    return 0;;
}

