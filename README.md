#include <stdio.h>
int fibonacci(int n) {
if (n <= 1)
return n;
return fibonacci(n - 1) + fibonacci(n - 2);
}
int main() {
int n = 10; // Number of Fibonacci numbers to generate
for (int i = 0; i < n; i++) {
printf("%d ", fibonacci(i));
}
return 0;
}
input;n=10
output=0 1 1 2 3 5 8 13 21 34 
