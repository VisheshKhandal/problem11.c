//  TODO: claculating the sum of 1 to n numbers in odd numbers

// #include<stdio.h>

// int main() {
//     int num;
//     int sum = 0;
//     printf("Enter a number: ");
//     scanf("%d", &num);

//     for (int i = 1; i <= num; i++) {
//         if (i % 2!= 0) {
//             sum = sum + i;
//         }
//     }
//     printf("The sum of 1 to %d odd numbers is: %d", num, sum);
//     return 0;
// }

//  TODO: calculate the sum of 1 to n numbers in even numbers

// #include<stdio.h>

// int main() {
//     int num;
//     int sum = 0;
//     printf("Enter a number: ");
//     scanf("%d", &num);

//     for (int i = 1; i <= num; i++) {
//         if (i % 2 == 0) {
//             sum = sum + i;
//         }
//     } 
//     printf("The sum of 1 to %d even numbers is: %d", num, sum); 
//     return 0;
// }                                  

// TODO: calculate the factorial of 1 to n numbers 

// #include<stdio.h>

// int main() {
//     int num;
//     printf("enter the number :");
//     scanf("%d", &num);

//     int i = 1;
//     int fact = 1;
//     while (i <= num) {
//         fact = fact * i;
//         i++;
//     }
//     printf("The factorial of %d is: %d", num, fact); 
//     return 0;
// } 

//  TODO: sum of digits of 1 to n numbers entered by the user 

// #include<stdio.h>

// int main() {
//     int num;
//     printf("enter the number :");
//     scanf("%d", &num);

//     int sum  = 0;
//     int copy = num;
//     while (num>0){
//         sum += num % 10;
//         num = num / 10;
//     }
//     printf("The sum of digits of %d is: %d", copy, sum);
//     return 0;
// } 

//  TODO: FIND LCM OF TWO NUMBERS ENTERED BY THE USER using TERNARY OPERATOR

// #include<stdio.h>

// int main() {
//     int first,second;
//     printf("Enter the first number: ");
//     scanf("%d", &first);

//     printf("Enter the second number: ");
//     scanf("%d", &second);

//     int min = (first > second)? first : second;
//     int max = first * second;
     
//     for (int i =min; i <= max; i++){
//         if (i % first == 0 && i % second == 0) {
//             printf("The LCM of %d and %d is: %d", first, second, i);
//             break;
//         }   
//     }
//     return 0;
// }

//  TODO: checking for prime numbers

// #include<stdio.h>

// int main() {
//     int num;
//     printf("Enter a number: ");
//     scanf("%d", &num);

//     for(int i = 2; i < num;i++){
//         if (num % i == 0) {
//             printf("%d is not a prime number", num);
//             return 0;
//         }   
//     }
//     printf("%d is a prime number", num);
//     return 0; 
// }

// TODO: reversing the nmber entered by the user

// #include<stdio.h>

// int main() {
//     int num;
//     printf("Enter a number: ");
//     scanf("%d", &num);

//     int reverse = 0;
//     int copy = num;
//     while(copy > 0){
//         reverse = (reverse * 10) + (copy % 10);
//         copy = copy / 10;   
//     }
//     printf("The reverse of %d is: %d", num, reverse);   

//     return 0;
// }

// TODO:  Armstrong number solve  

// #include<stdio.h>

// int main() {
//     int num;
//     printf("Enter a number: ");
//     scanf("%d", &num);

//     int sum = 0;
//     int copy = num;
//     while(copy > 0){
//         int digit = copy % 10;
//         sum = sum + (digit * digit * digit);
//         copy = copy / 10;
//     }   
//     if(sum == num){
//         printf("%d is an Armstrong number", num);   
//     }
//     else{
//         printf("%d is not an Armstrong number", num);   
//     }   
//     return 0;
// }

//  TODO: FINDING THE PALINDROME OF THE NUMBERS 
// #include<stdio.h>

// int main() {
//     int num;
//     printf("Enter a number: ");
//     scanf("%d", &num);

//     int reverse = 0;
//     int copy = num;
//     while(copy > 0){
//         reverse = (reverse * 10) + (copy % 10);
//         copy = copy / 10;   
//     }
//     if(reverse == num){
//         printf("%d is a palindrome number", num);
//     }
//     else{
//         printf("%d is not a palindrome number", num);   
//     }
//     return 0;
// }

// TODO: when user entered the 0 then print the sum before we entered number
// #include<stdio.h>

// int main() {
//     int sum;
//     int num;
//     do{
//         printf("Enter a number: ");
//         scanf("%d", &num);
//         sum += num;
//     }while (num != 0);

//     printf("The sum is: %d", sum);  
//     return 0;
// }

//TODO: print th square of number ana entered -1 then stop the program

// #include<stdio.h>

// int main() {
//     int num;
//     printf("enter the number : ");
//     scanf("%d", &num);
//     while(1){
//          printf("The square of %d is: %d\n", num, num * num);
//          printf("Enter -1 to stop the program: ");
//          scanf("%d", &num);
//          if(num == -1){
//              break;
//              printf("The program is stopped");  
//          }
       
//     } 

//     return 0;
// }
//  TODO:  pascle triangle
#include <stdio.h>

int main() {
    int rows, i, j, coefficient = 1;

    printf("Enter the number of rows: ");
    scanf("%d", &rows);

    for (i = 1; i <= rows; i++) {
         
        for (int space = 1; space <= rows - i; space++) {
            printf("  "); // Two spaces for better formatting
        }

        for (j = 1; j <= i; j++) {
            printf("%d  ", coefficient);
            coefficient = coefficient * (i - j + 1) / j;
        }

        printf("\n");
    }

    return 0;
}

 
