#include<stdio.h>
#include<strings.h>
struct employee{
   	char name[20];
   	char edu[15];
	char profession[12];
	char available_days[12];
	char contact[20];   //this can either be your e mail or phone no
	int pay_per_hour;
	char work_experince[10];
	char availible_hours[15];
};
struct customer{
	char service1[10];
	char service2[10];
	char service3[10];
	char service4[10];
	char service5[10];
};
int main(){
	struct employee n[100];
	int choice,a,i=0;
	printf("\t\t\t-------------------------------------------");
	printf("\n\t\t\t*<<<*<<<*<<<*<<<* JABBO *>>>*>>>*>>>*>>>");
	printf("\n\t\t\t-------------------------------------------");
	printf("\nMAKING LIFE EASIER\n");
	while(choice!=3){
	 printf("1.Customer\n2.Employee\n3.exit\nEnter Your Choice:");
    scanf("%d",&choice);
	if(choice==1){
    	printf("1.electrician\n2.cleaner\n3.plumber\n4.mechanic\n5.carpenter\nenter your choice: ");
    	scanf("%d",&a);
		 //printf("%d\n",n[i].pay_per_hour);
        if(a==1){
        	for(int j=0;j<100;j++){
        		if(strcmp(n[j].profession,"electrician")==0){
        			//printf("c");
        			printf("----HERE IS YOUR MATCHED RESULT----\n");
        			printf("name: %s\n",n[j].name);
        			printf("your contact: %s\n",n[j].contact);
        			printf("pay per hour: %d\n",n[j].pay_per_hour);
        			printf("work experience: %s\n",n[j].work_experince);
        			printf("available days: %s\n", n[j].available_days);
        			printf("available hours: %s\n", n[j].availible_hours);
				}
				
				
				}
			}
		 else if(a==2){
				for(int j=0;j<100;j++){
				 if(strcmp(n[j].profession,"cleaner")==0){
				 	printf("----HERE IS YOUR MATCHED RESULT----\n");
					printf("name:%s\n",n[j].name);
        			printf("your contact: %s\n",n[j].contact);
        			printf("pay per hour: %d\n",n[j].pay_per_hour);
        			printf("work experience: %s\n",n[j].work_experince);
        			printf("available days: %s\n", n[j].available_days);
        			printf("available hours: %s\n", n[j].availible_hours);
				}
				}
			}
			else if(a==3){
			    for(int j=0;j<100;j++){
					if(strcmp(n[j].profession,"plumber")==0){
					printf("----HERE IS YOUR MATCHED RESULT----\n");
					printf("name:%s\n", n[j].name);
        			printf("your contact: %s\n", n[j].contact);
        			printf("pay per hour: %d\n", n[j].pay_per_hour);
        			printf("work experience: %s\n", n[j].work_experince);
        			printf("available days: %s\n", n[j].available_days);
        			printf("available hours: %s\n", n[j].availible_hours);
				}
			}
			}
			   else if(a==4){
			        for(int j=0;j<100;j++){
					 if(strcmp(n[j].profession,"mechanic")==0){
					printf("\t----HERE IS YOUR MATCHED RESULT----\n");
					printf("name:%s\n",n[j].name);
        			printf("your contact: %s\n",n[j].contact);
        			printf("pay per hour: %d\n",n[j].pay_per_hour);
        			printf("work experience: %s\n",n[j].work_experince);
        			printf("available days: %s\n", n[j].available_days);
        			printf("available hours: %s\n", n[j].availible_hours);
				}
				}}
				else if(a==5){
			        for(int j=0;j<100;j++){
					 if(strcmp(n[j].profession,"carpenter")==0){
					printf("----HERE IS YOUR MATCHED RESULT----\n");
					printf("name:%s\n",n[j].name);
        			printf("your contact: %s\n",n[j].contact);
        			printf("pay per hour: %d\n",n[j].pay_per_hour);
        			printf("work experience: %s\n",n[j].work_experince);
        			printf("available days: %s\n", n[j].available_days);
        			printf("available hours: %s\n", n[j].availible_hours);
				}
				}
				}
	
	}
	else if(choice==2){
	  printf("\t\t\t#### FORM OF EMPLOY #####\n");
	  printf("Enter Your Profession name: ");
	  fflush(stdin);
	  scanf("%s",n[i].profession);
	  //printf("%s\n",n[i].profession);
	  printf("Enter Your Name: ");
	  fflush(stdin);
	  gets(&n[i].name);
	  fflush(stdin);
	  printf("enter your education: ");
	  gets(&n[i].edu);
	  fflush(stdin);
	  printf("available days: ");
	  gets(&n[i].available_days); 
	  fflush(stdin);
	  printf("available hours: ");
	  gets(&n[i].availible_hours);
	  fflush(stdin);
	  printf("Enter Your contact:");
	  gets(&n[i].contact);
	  fflush(stdin);
	  printf("Enter Your Pay Per Hour: ");
	  scanf("%d",&n[i].pay_per_hour);
	  fflush(stdin);
	  printf("Enter Your Experince: ");
	  gets(&n[i].work_experince);  
	  i++;
	}
	else{
		//printf("Wrong choice");
	}

}
}
