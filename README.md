# ovsiyenko_lab5
#include <stdio.h>

int main() {
    int array[10], max, min;

    printf("Введіть 10 чисел:\n");
    for (int i = 0; i < 10; i++) {
        scanf("%d", &array[i]);
    }

    max = min = array[0];
    for (int i = 1; i < 10; i++) {
        if (array[i] > max) max = array[i];
        if (array[i] < min) min = array[i];
    }

    printf("Різниця: %d\n", max - min);
    return 0;
}
