```
#include<conio.h>
#include<stdio.h>
#include<string.h>
void main() {
	/*variable declaration part */
	int rl,s1,s2,s3,s4,s5,s6,t;
	float per;
	char nm[25],div[10];
	/*reading part */
	printf("Enter the Roll No : ");
	scanf("%d",&rl);
	printf("Enter Name        : ");
	fflush(stdin);
	gets(nm);
	printf("Enter six Subject Marks :\n");
	scanf("%d%d%d%d%d%d",&s1,&s2,&s3,&s4,&s5,&s6);
	/* processing part */
	t=s1+s2+s3+s4+s5+s6;
	per=t/6.0;
	if(per>=75)
	     strcpy(div,"Honour"); else if( per>=60)
		  strcpy(div,"First"); else if( per>=48)
			 strcpy(div,"Second"); else if (per>=36)
			     strcpy(div,"Pass"); else
			     strcpy(div,"Fail");
	/* display part */
	printf("\t\tSt.peters christu jyothi school\n");
	printf("\n\n");
	printf("Roll No: %d \t  Name : %s\n",rl,nm);
	printf("---------------------------------------------------\n");
	printf("Subject             Max      Min            Obt.Marks\n");
	printf("---------------------------------------------------\n");
	printf("Telugu                100      36              %d\n",s1);
	printf("Hindi              100      36              %d\n",s2);
	printf("English               100      36              %d\n",s3);
     printf("Maths              100      36              %d\n",s3);
     printf("Science             100      36              %d\n",s3);
     printf("Social            100      36              %d\n",s3);
 printf("---------------------------------------------------\n");
	printf("				  Total          %d\n",t);
	printf("per  %f\t\t\t  div: %s \n",per,div);
	printf("---------------------------------------------------\n");
	getch();
}
  ```
