# #include <stdio.h>
#include <stdlib.h>

int main() {
    char ch;
    double a, b;

    while (1) {
        printf("Operator select (+, -, *, /), or 'x' to quit: ");
        scanf(" %c", &ch);

        if (ch == 'x')
            exit(0);

        printf("Enter two operands: ");
        scanf("%lf %lf", &a, &b);

        switch (ch) {
            case '+':
                printf("%.1lf + %.1lf = %.1lf\n", a, b, a + b);
                break;
            case '-':
                printf("%.1lf - %.1lf = %.1lf\n", a, b, a - b);
                break;
            case '*':
                printf("%.1lf * %.1lf = %.1lf\n", a, b, a * b);
                break;
            case '/':
                printf("%.1lf / %.1lf = %.1lf\n", a, b, a / b);
                break;
            default:
                printf("Error! Please write a valid operator.\n");
        }
        printf("\n");
    }
    return 0;
}

This is  my first git report
