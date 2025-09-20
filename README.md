#include <stdio.h>

int main() {
    int n, i;

    // Input array size
    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int arr[n]; // Declare array

    // Input array elements
    printf("Enter %d elements:\n", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    // Assume first element is maximum
    int max = arr[0];

    // Compare with the rest
    for (i = 1; i < n; i++) {
        if (arr[i] > max) {
            max = arr[i];
        }
    }

    // Output result
    printf("Maximum element: %d\n", max);

    return 0;
}
