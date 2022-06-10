# powerseries
#include<stdio.h>

int pow(int a, int b){
	if(b>=1){
		if(a>=1){
			return a*pow(a,b-1);
		}
	}
	else{
		return 1;
	}
}

int main()
{
	int n; int i;
	printf("Enter the number\n");
	scanf("%d",&n);
	printf("Enter the power\n");
	scanf("%d",&i);
	printf("The %d to the power %d is %d",n,i,pow(n,i));
	return 0;
}
