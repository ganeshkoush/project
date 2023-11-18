
#include<stdio.h>
#include<stdlib.h>
#define bonous 2000
struct employee{
	
	char name[40];
	int id;
	float basic_salary;
	float net_salary;
};
void main(){
	
	int n,i;
	
	printf("\nenter how many employes data should be entered:");
    scanf("%d",&n);
    
    struct employee emp[n];
    
    printf("\nplease enter the details %d employe's",n);
    for(i=0;i<n;i++){
    	printf("\nenter details of employee %d",i+1);
    	
    	printf("\nenter name:");
    	scanf("%s",emp[i].name);
    	
    	printf("enter id:");
    	scanf("%d",&emp[i].id);
    	
    	printf("enter basic salary:");
    	scanf("%f",&emp[i].basic_salary);
    	
    	emp[i].net_salary=emp[i].basic_salary+bonous;
    	
	}
	
	printf("########## All Employees Details ##########\n");
    for(i=0; i<n; i++){
 
        printf("Name of the employee:-");
        printf("%s \n",emp[i].name);
 
        printf("Id:-");
        printf("%d \n",emp[i].id);
 
        printf("Salary:-");
        printf("%f \n",emp[i].net_salary);
        
        
 
        printf("\n");
       
    }
    
    printf("########## THE END ##########"); 
 
	
	
}
