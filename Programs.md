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




























































