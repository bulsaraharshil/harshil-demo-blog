---
title: Bubble Sort in C
date: "2020-04-09T22:12:03.284Z"
description: "I am going to show program of Bubble Sort in C "
---

#include<stdio.h>
#include<conio.h>

void bubblesort(int a[],int n);
void main()
{
int i,n,a[20];
printf("enter elements");
scanf("%d",&n);
printf("enter value of elements");
for(i=0;i<n;i++)
scanf("%d",&a[i]);
bubblesort(a,n);
for(i=0;i<n;i++)
printf("%d ",a[i]);
getch();
}

void bubblesort (int a[],int n)
{
int i,j,temp;
for(i=n-1;i>0;i--)
{
for(j=0;j<i;j++)
{
if (a[j]>a[j+1])
{
temp=a[j];
a[j]=a[j+1];
a[j+1]=temp;
}
}
}
}
