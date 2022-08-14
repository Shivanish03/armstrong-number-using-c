/*# armstrong-number-using-c*/
#include<stdio.h>
#include<conio.h>
int main()
{
//armstrong number is:-153=1*1*1+5*5*5+3*3*3
int num,onum,rem,res=0;
printf("enter the three digit number:-");
scanf("%d",&num);
onum=num;
while(onum!=0)
{
rem=onum%10;
res+=rem*rem*rem;
onum/=10;
}
if(res==num)
printf("%d is an armstrong number." ,num);
else
printf("%d is not an armstrong number." , num);
return 0;
}
