#include <stdio.h>

// Function to calculate factorial iteratively
unsigned long long factorial_iterative(int n) {
    if (n < 0) return 0; // Error handling for negative input
    
    unsigned long long result = 1;
    while (n > 1) {
        result *= n;
        n--;
    }
    return result;
}

int main() {
    int num = 5;
    printf("Factorial of %d (Iterative) is: %llu\n", num, factorial_iterative(num));
    return 0;
}
