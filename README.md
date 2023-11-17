#include<stdio.h>
struct employee{
	
	char name[40];
	int id;
	float basic_salary;
	float net_salary
};
void main(){
	
	int n,i;
	
	printf("\n enter how many employes data should be entered");
    scanf("%d",&n);
    
    struct employee emp[n];
    
    printf("\n employee details %d",n);
    for(i=0;i<n;i++){
    	
    	printf("\n enter name");
    	scanf("%s",emp[i].name);
    	
    	printf("\n enter id");
    	scanf("%d",&emp[i].id);
    	
    	printf("\n enter basic salary");
    	scanf("%f",&emp[i].basic_salary);
    	
    	emp[i].net_salary=emp[i].basic_salary+20000;
    	
	}
	
	printf(" ############# All Employees Details ############# \n");
    for(i=0; i<n; i++){
 
        printf("Name:\t: ");
        printf("%s \n",emp[i].name);
 
        printf("Id:\t: ");
        printf("%d \n",emp[i].id);
 
        printf("Salary:\t: ");
        printf("%f \n",emp[i].net_salary);
        
        
 
        printf("\n");
    }
 
	
	
}
