# bubble-sort.c
//(BUBBLE SORT) C program to print array in ascending order using bubble sort method.
//(BUBBLE SORT) C program to print array in ascending order using bubble sort method.


#include <stdio.h>

int main() {
    int i,j,t,flag;
    int a[]={5,4,3,2,1};
    printf("array of 5 elements is created:\n");
    for(i=0;i<5;i++)
    printf("%d\n",a[i]);
    
    for(i=0;i<4;i++)
     for(j=0;j<=3-i;j++)
      if(a[j]>a[j+1]){
          t=a[j];
          a[j]=a[j+1];
          a[j+1]=t;
      }
     printf("Array after bubble sorting is=\n");
     for(i=0;i<5;i++)
      printf("%d\n",a[i]);
    return 0;
}
