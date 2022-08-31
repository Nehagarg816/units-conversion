# units-conversion
This is a program for conversion of some units into one another using switch case.


#include<stdio.h>
#include<conio.h>
void main()
{
	char input;
	float a,b;
	printf("Press 1 for km to miles");
	printf("\nPress 2 for inches to foot");
	printf("\nPress 3 for cm to inches");
	printf("\nPress 4 for pounds to kg");
	printf("\nPress 5 for inches to meters");
	printf("\nPress q to break");
	printf("\nEnter your choice:");
	scanf("%c",&input);
	
	switch(input)
	{
		case '1':
			printf("\nEnter one value in km :");
			scanf("%f",&a);
			b=0.621371*a;
			printf("Value of given number in miles is %f",b);
			break;
			
		case '2':
			printf("\nEnter one value in inches :");
			scanf("%f",&a);
			b=0.0833333*a;
			printf("Value of given number in foot is %f",b);
			break;
			
		case '3':
			printf("\nEnter one value in cms :");
			scanf("%f",&a);
			b=0.393701*a;
			printf("Value of given number in inches is %f",b);
			break;
			
		case '4':
			printf("\nEnter one value in pounds :");
			scanf("%f",&a);
			b=0.453592*a;
			printf("Value of given number in kg is %f",b);
			break;
			
		case '5':
			printf("\nEnter one value in inches :");
			scanf("%f",&a);
			b=0.0254*a;
			printf("Value of given number in metres is %f",b);
			break;
			
		case 'q':
			printf("Invalid input");
			printf("\nQuitting the program");
			break;
	}
}
