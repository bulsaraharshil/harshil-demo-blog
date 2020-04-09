---
title: Swap 2 numbers without using 3rd variable in C
date: "2020-04-09T22:40:32.169Z"
description: I am going to show how to swap 2 numbers without using 3rd variable
---

#include<stdio.h>
int main()  
{  
int a=10, b=20;  
printf("Before swap a=%d b=%d",a,b);  
//This is main logic
a=a+b;//a=30 (10+20)  
b=a-b;//b=10 (30-20)  
a=a-b;//a=20 (30-10)  
printf("\nAfter swap a=%d b=%d",a,b);  
return 0;  
}
