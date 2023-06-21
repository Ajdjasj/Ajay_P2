# Prgrm-for-STM

//enum
#include<stdio.h>
#include<string.h>
void main()
{
	char str[30];
	int len,i,temp;
	printf("Enter string: ");
	gets(str);
	len=strlen(str);
	for(i=0;i<(len/2);i++)
	{
		temp=str[i];
		str[i]=str[len-i-1];
		str[len-i-1]=temp;
	}
	printf("%s\n",str);
 }