# The FizzBuzz Game

```C
#include <stdio.h>

int main() {
    int i, n;
    printf("Enter n: ");
    scanf("%d", & n);

    if (n % 3 == 0 && n % 5 == 0) {
        printf("FizzBuzz");
    } else if (n % 3 == 0) {
        printf("Fizz");
    } else if (n % 5 == 0) {
        printf("Buzz");
    }
    return 0;
}
```

# In or Out

```C
#include <stdio.h>

int main() {

    int n;
    printf("Enter n: ");
    scanf("%d", & n);

    if (n % 2 == 0) {
        printf("In");
    } else {
        printf("Out");
    }

    return 0;
}
```


# Where's the Biggest One?
```C
#include <stdio.h>

int main() {

    int first, second, third, fourth, fifth;

    printf("Enter integer 1: ");
    scanf("%d", & first);

    printf("Enter integer 2: ");
    scanf("%d", & second);

    printf("Enter integer 3: ");
    scanf("%d", & third);

    printf("Enter integer 4: ");
    scanf("%d", & fourth);

    printf("Enter integer 5: ");
    scanf("%d", & fifth);

    // int arr1 = {first, second, third, fourth, fifth};
    // int arr2 = {first, second, third, fourth, fifth};

    if (first > second && first > third && first > fourth && first > fifth) {
        printf("Leftmost");
    } else if (third > first && third > second && third > fourth && third > fifth) {
        printf("Middle");
    } else if (fifth > first && fifth > second && fifth > third && fifth > fourth) {
        printf("Rightmost");
    } else {
        printf("Unknown");
    }

    return 0;
}
```

# The Positive Ones
```C
#include<stdio.h>

int main() {

    float a, b, c, d;

    printf("Enter the first number: ");
    scanf("%f", & a);
    printf("Enter the second number: ");
    scanf("%f", & b);
    printf("Enter the third number: ");
    scanf("%f", & c);
    printf("Enter the fourth number: ");
    scanf("%f", & d);

    float total = 0;
    if (a > 0) {
        total = total + 1;
    }
    if (b > 0) {
        total = total + 1;
    }
    if (c > 0) {
        total = total + 1;
    }
    if (d > 0) {
        total = total + 1;
    }
    printf("Count of positives = %.0f\n", total);
}

}
```

# Jackpot!
```c
#include<stdio.h>

int main() {
    int num1, num2;

    printf("Enter the 3-digit integer: ");
    scanf("%d", & num1);
    printf("Enter the digit to be searched (0 - 9): ");
    scanf("%d", & num2);

    if (num2 == num1 % 10 && num2 == num1 / 10 % 10 && num2 == num1 / 100 % 10) {
        printf("Jackpot!");
    } else {
        printf("Nah");
    }
    return 0;
}
```

# The Greater One
```c
#include <stdio.h>

int main() {

    float first, second;

    printf("Enter the first number: ");
    scanf("%f", & first);

    printf("Enter the second number: ");
    scanf("%f", & second);

    if (first > second) {
        printf("Greater");
    } else {
        printf("Lesser");
    }

    return 0;
}
```

# Is It You, Cody?
```C
#include<stdio.h>

int main(void) {
    char var1, var2, var3, var4;

    printf("Enter the first character: ");
    scanf("%c", & var1);
    printf("Enter the second character: ");
    scanf(" %c", & var2);
    printf("Enter the third character: ");
    scanf(" %c", & var3);
    printf("Enter the fourth character: ");
    scanf(" %c", & var4);

    if (var1 == 'C' || var1 == 'c') {
        if (var2 == 'O' || var2 == 'o') {
            if (var3 == 'D' || var3 == 'd') {
                if (var4 == 'Y' || var4 == 'y')
                    printf("Correct");
                else printf("Wrong");
            } else printf("Wrong");
        } else printf("Wrong");
    } else printf("Wrong");

    return 0;

}
```