#include <stdio.h>
int linearSearch(int arr[], int n, int key) {
for (int i = 0; i < n; i++) {
if (arr[i] == key) {
return i;  // Return the index if key is found
}
}
return -1;  // Return -1 if key is not found
}
int main() {
int arr[] = {12, 45, 78, 23, 56};
int n = sizeof(arr) / sizeof(arr[0]);
int key = 78;
int result = linearSearch(arr, n, key);
if (result != -1) {
printf("Element found at index: %d", result);
} else {
printf("Element not found");
}
return 0;
}
output:found element at index at 2
