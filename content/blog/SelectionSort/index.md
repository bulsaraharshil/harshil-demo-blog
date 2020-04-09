---
title: Selection Sort in C
date: "2020-04-09T22:12:03.284Z"
description: "I am going to show program of Selection Sort in C "
---

#include<stdio.h>
#include<conio.h>
void selectionsort(int a[],int n);
void main()
{
int n,i,a[10];
clrscr();
printf("enter the no of elements");
scanf("%d",&n);
printf("enter the elements");
for(i=0;i<n;i++)
scanf("%d",&a[i]);
selectionsort(a,n);
for(i=0;i<n;i++)
printf("%d",a[i]);
getch();
}
void selectionsort(int a[],int n)
{
int i,j,index,large;
for(i=n-1;i>0;i--)
{
large=a[0];
index=0;
for(j=1;j<=i;j++)
{
if (a[j]>large)
{
large=a[j];
index=j;
}
}
a[index]=a[i];
a[i]=large;
}
}
