void printFibonacci(int n) {
    int first = 0, second = 1, next;
    printf("Fibonacci Series: ");
    for (int i = 0; i < n; i++) {
        if (i == 0) {
            printf("%d ", first);
        } else if (i == 1) {
            printf("%d ", second);
        } else {
            next = first + second;
            first = second;
            second = next;
            printf("%d ", next);
        }
    }
    printf("\n");
}
