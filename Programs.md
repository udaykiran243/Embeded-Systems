# ARRAYS
## Write a program in C to store elements in an array and print them.
```c
#include<stdio.h>
int main(){
    int arr[] = {10,20,30,40};
    int size = sizeof(arr)/ sizeof(arr[0]);
    for(int i = 0; i < size; i++) printf("%d ", arr[i]);
}
```
## Write a program in C to count the total number of duplicate elements in an array.
```c
#include<stdio.h>
int main(){
    int arr[] = {1,23,5,2,4,5,1},n, count = 0;
    n = sizeof(arr)/sizeof(arr[0]);
    int dep[n];
    for(int i = 0 ;i < n; i++){
        dep[i] = 1;
    }
    for(int i = 0; i < n; i++){
        for(int j = i+1; j < n; j++){
            if(arr[i] != 0 && arr[i] == arr[j]){
                dep[i]++;
                arr[j] = 0; 
            }
        }
    }
    for(int i = 0; i < n; i++){
        if(arr[i] != 0)
        printf("%d is repeated %d times\n", arr[i], dep[i]);
    }
}
```
## Write a program in C to print all unique elements in an array.
```c
#include<stdio.h>
int main(){
    int arr[] = {1,23,5,2,4,5,1},n, count = 0;
    n = sizeof(arr)/sizeof(arr[0]);
    int dep[n];
    for(int i = 0 ;i < n; i++){
        dep[i] = 1;
    }
    for(int i = 0; i < n; i++){
        for(int j = i+1; j < n; j++){
            if(arr[i] != 0 && arr[i] == arr[j]){
                dep[i]++;
                arr[j] = 0; 
            }
        }
    }
    for(int i = 0; i < n; i++){
        if(dep[i] == 1 && arr[i] != 0)
        printf("%d is a unique element\n", arr[i]);
    }
}
```
# POINTERS
## 1. Write a Program to print the address of variables using the address operator and print size of pointer variables and size of values Dereferenced by them and illustrate the dereferencing of pointers.
```c
#include<stdio.h>
int main(){
    int val = 10;
    int *p = &val;
    printf("%p\n", &val);
    printf("%d\n", sizeof(p));
    printf("%d\n", sizeof(*p));
}
```
## C program to illustrate pointer arithmetic
```c
#include<stdio.h>
int main(){
    int val = 10;
    int *p = &val;
    printf("%d", *p+1);
}
```
## Program to print the values and address of elements of 2-d array.
```c
#include<stdio.h>
int main(){
    int arr[][2] = {{10,20},{30,40}};
    int (*p)[2];
    p = arr;
    for(int i = 0; i < 2; i++){
        for (int j=0; j < 2; j++){
            printf("%d  %p\n", *(*(p+i)+j), ((p+i)+j));
        }        
    } 
}
```
## Program to print elements of a 2-D array by subscripting a pointer to an array variable.
```c
#include<stdio.h>
int main(){
    int arr[][2][2] = {
        {10,20},{30,50},
        {1,2},{3,4},
    };
    int (*p)[2][2];
    p = arr;
    for(int i = 0; i < 2; i++){
        for(int j = 0 ; j < 2 ; j++){
            for(int k = 0; k < 2; k++){
                printf("%d ", *(*(*(p+i)+j)+k));
            }
        }
    }
}
```
## Write a program to pass a 1D array to a function.
```c
#include<stdio.h>
int fun(int *p){
    *(p+1) = 100;
}
int main(){
    int arr[] = {10,20,30,40,50};
    printf("%d ", arr[1]);
    fun(arr);
    printf("%d ", arr[1]);
}
```
## Create a function that swaps two numbers using pointers.
```c
#include<stdio.h>
int fun(int *p,int *p1){
    int temp = *p;
    *p = *p1;
    *p1 = temp;
}
int main(){
   int a = 10, b =20;
   printf("%d %d\n", a, b);
   fun(&a, &b);
   printf("%d %d\n",a,b);
}
```
## Develop a function to reverse a string in place using pointers.
```c
#include<stdio.h>
#include<string.h>
int fun(char *p){
    printf("%s", p);
    int i = strlen(p)-1, j =0;
    while (j < i)
    {
        char temp = *(p+i);
        *(p+i) = *(p+j);
        *(p+j) = temp;
        i--;
        j++;
        /* code */
    }
    printf("%s\n", p);
    
}
int main(){
   char str[] = "hello";
   fun(str);
   printf("%s",str);
}
```
## Implement a function to copy one string into another using pointers, without using any standard library functions.
```c
#include<stdio.h>
int main(){
    char str[] = "hello";
    printf("%s", str);
    char *p = str;
    printf("%s", p);
    char p1[6];
    for(int i = 0; i < 6; i++){
        *(p1+i) = *(p+i);
    }
    printf("%s",p1);
}
```
## Write a program to compare two strings lexicographically (like the strcmp function) using pointers.
```c
#include<stdio.h>
int main(){
    printf("enter the string :");
    char str[5];
    scanf("%s",str); printf("%s", str);

    printf("enter the second string :");
    char str1[5];
    scanf("%s", str1);

    char *p = str, *p1 = str1;

    int  i = 0;
    while(*(p+i) != '\0'){
        if(*(p+i) == *(p1+i)) i++;
        else break; 
    }

    if(*(p+i) == '\0' && *(p1+i)== '\0')  printf("The Strings %s and %s are lexicographically equal", str,str1);
    else printf("The Strings %s and %s are not lexicographically equal", str ,str1);

}
```
## Write a program to find the largest element using Dynamic Memory Allocation.
```c
#include<stdio.h>
#include<stdlib.h>
int main(){
    int *p = (int *)malloc(sizeof(int) * 1);
    int *p1 = (int *)malloc(sizeof(int) * 1);
    *p = 5;
    *p1 = 6;
    if(*p > *p1) printf("%d is greater than %d", *p, *p1);
    else printf("%d is greater than %d", *p1, *p);
}
```
## Write a program to show a pointer to an array whose contents are pointers to structures.
```c
#include<stdio.h>
#include<stdlib.h>
struct ARRAY{
    int data;
    char name[100];
};
int main(){
  struct ARRAY p = { 10, "Uday"};  
  struct ARRAY p2 = { 20, "Sai"};
  struct ARRAY arr[] = {p,p2};
  struct ARRAY *ptr = arr;
  for (int i = 0; i < 2; i++)
  {
    printf("Name = %s and Data = %d\n", (ptr+i) -> name , (ptr+i)->data);
    /* code */
  }
    
}
```
## Write a program to add two matrices using pointers.
```c
#include <stdio.h>

#define ROW 2
#define COL 2

int main() {
    int A[ROW][COL] = {{1, 2}, {3, 4}};
    int B[ROW][COL] = {{5, 6}, {7, 8}};
    int C[ROW][COL];

    int *pA = &A[0][0];
    int *pB = &B[0][0];
    int *pC = &C[0][0];

    for (int i = 0; i < ROW * COL; i++) {
        *(pC + i) = *(pA + i) + *(pB + i);
    }

    // Display result
    printf("Matrix Addition Result:\n");
    for (int i = 0; i < ROW; i++) {
        for (int j = 0; j < COL; j++) {
            printf("%d ", C[i][j]);
        }
        printf("\n");
    }

    return 0;
}
```
## Write a program to multiply two matrix using pointers
```c
#include <stdio.h>

#define ROW 2
#define COL 2

int main() {
    int A[ROW][COL] = {{1, 2}, {3, 4}};
    int B[ROW][COL] = {{5, 6}, {7, 8}};
    int C[ROW][COL] = {0};

    int *pA = &A[0][0];
    int *pB = &B[0][0];
    int *pC = &C[0][0];

    for (int i = 0; i < ROW; i++) {
        for (int j = 0; j < COL; j++) {
            for (int k = 0; k < COL; k++) {
                *(pC + i * COL + j) += *(pA + i * COL + k) * *(pB + k * COL + j);
            }
        }
    }

    // Display result
    printf("Matrix Multiplication Result:\n");
    for (int i = 0; i < ROW; i++) {
        for (int j = 0; j < COL; j++) {
            printf("%d ", C[i][j]);
        }
        printf("\n");
    }

    return 0;
}
```




























































