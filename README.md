# Headspin-assignment
//Program to convert binary to decimal



#include <stdio.h>
 

void main()

{
    
	int  a, bin, dec = 0, base = 1, rem,i;
 
   
	printf("Enter a binary number \n");
                 //Enter the binary number
	scanf("%d", &a); 
                                   
	bin = a;
    
	do
    
	{
        
		rem = a % 10;
        
		dec = dec + rem * base;
        
		a = a / 10 ;
        
		base = base * 2;
    
	}while(a>0);
                                             
	printf("Its decimal equivalent of %d is = %d \n",bin,dec);

}
    
