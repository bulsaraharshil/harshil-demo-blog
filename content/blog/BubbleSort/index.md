---
title: Bubble Sort in C
date: "2020-04-09T22:12:03.284Z"
description: "I am going to show program of Bubble Sort in C "
---

#include<stdio.h>

int main(){

int count, temp, i, j, number[30];

printf("How many numbers are u going to enter?: ");
scanf("%d",&count);

printf("Enter %d numbers: ",count);

for(i=0;i<count;i++)
scanf("%d",&number[i]);

/_ This is the main logic of bubble sort algorithm
_/
for(i=count-2;i>=0;i--){
for(j=0;j<=i;j++){
if(number[j]>number[j+1]){
temp=number[j];
number[j]=number[j+1];
number[j+1]=temp;
}
}
}

printf("Sorted elements: ");
for(i=0;i<count;i++)
printf(" %d",number[i]);

return 0;
}
