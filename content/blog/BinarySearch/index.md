---
title: Binary Search in C
date: "2020-04-09T22:12:03.284Z"
description: "I am going to show program of Binary Search in C "
---

#include<stdio.h>
#include<conio.h>
int bin_search(int k[],int n,int key);
int main()
{
int n,i,k[20],m,key;
printf("\n enter total no of elements");
scanf("%d",&n);
for(i=0;i<n;i++)
{
printf("\n Enter elements in array");
scanf("%d",&k[i]);
}
printf("\n enter no which u want to search");
scanf("%d",&key);
m=bin_search(k,n,key);
if(m==-1)
{
printf("\n element is not found");
}
else
{
printf("element is at position %d",m);
}
getch();
return 0;
}
int bin_search(int a[],int n,int key)
{
int m;
int mid;
int low=0;
int high=n-1;
while(low<high)
{
mid=(low+high)/2;
if(key==a[mid])
return mid;
if(key<a[mid])
high=m-1;
else
low=m+1;
}
return -1;
}
