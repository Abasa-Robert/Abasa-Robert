#include<stdio.h>
#include<string.h>
int main()
{
    struct student
    {
        char first_name[20];
        char last_name[15];
        char hall[25];
        int age;
    };
    struct student student1;
    char st_first_name[20], st_last_name[15], st_hall[15];
    int age;
    printf("Enter your first name\n");
    fgets(st_first_name,20,stdin);
    strcpy(student1.first_name, st_first_name);
    printf("Enter your second name\n");
    fgets(st_last_name,15,stdin);
    strcpy(student1.last_name, st_last_name);
    printf("Enter your hall of residence\n");
    fgets(st_hall,25,stdin);
    strcpy(student1.hall, st_hall);
    printf("Enter your age\n");
    scanf("%d",&age);
    printf("FIRST NAME: %s\n", student1.first_name);
    printf("LAST NAME: %s\n", student1.last_name);
    printf("FULL NAME: %s", strcat(student1.first_name,student1.last_name));
    printf("HALL: %s\n", student1.hall);
    printf("AGE: %d", age);
    
    
    
    
    
    return 0;
}
