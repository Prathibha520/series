#include <stdio.h>
#include <math.h>
void printFibonacci(int);
int isPrime(int);
long long powerOfXtoX(int);
int main() {
   int n, x,z;
   printf("Enter 1-Fibonnaci series \n 2-prime series \n 3-xpower series\n");
   printf("Enter the choice\n");
   scanf("%d",&z);
   switch (z)
   {
   case 1:
    printf("Enter the number of terms for Fibonacci series: ");
    scanf("%d", &n);
    printFibonacci(n);
    break;
    case 2:
    printf("Enter a number to check if it's prime: ");
    scanf("%d", &n);
    if (isPrime(n)) 
    {
        printf("%d is a prime number.\n", n);
    }
    else 
    {
        printf("%d is not a prime number.\n", n);
    }
    break;
    case 3:
    printf("Enter a number to calculate x^x: ");
    scanf("%d", &x);
    printf("%d^%d = %lld\n", x, x, powerOfXtoX(x));
    break;
    }
    return 0;
}
