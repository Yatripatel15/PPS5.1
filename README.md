# PPS5.1
About odd numbers and their sum
#include <stdio.h>

int main() 
{
    int n, sum = 0;

    // Asking for input
    printf("Enter the number of terms: ");
    scanf("%d", &n);

    printf("The first %d odd natural numbers are: \n", n);

    // Loop to display odd numbers and calculate the sum
    for(int i = 1, count = 0; count < n; i++) {
        if(i % 2 != 0)
        {
            printf("%d ", i);
            sum += i;
            count++;
        }
    }

    // Display the sum
    printf("\nSum of odd natural numbers = %d\n", sum);

    return 0;
}

