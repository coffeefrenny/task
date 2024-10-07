#include <stdio.h>
#include <stdlib.h>


int main() {
    char correct_password[] = "vikings";
    char input[10];
    int access_granted = 0;

    do {
        printf("Enter your password: ");
        scanf("%9s", input);

    if (strcmp(input, correct_password) == 0) {
        printf("Access has been granted!\n");
        access_granted = 1;
    } else {
    printf("Your password is incorrect. Think again.\n");
        }
    } while (!access_granted);

    return 0;
