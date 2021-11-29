# Section 3 - React Basics
<hr>

```C
#include<stdio.h>

int main(void){
    int num1,num2,num3,num4,num5;

    printf("Enter integer 1: ");
    scanf("%d", &num1);
    printf("Enter integer 2: ");
    scanf("%d", &num2);
    printf("Enter integer 3: ");
    scanf("%d", &num3);
    printf("Enter integer 4: ");
    scanf("%d", &num4);
    printf("Enter integer 5: ");
    scanf("%d", &num5);

    if(num1 > num2 && num1 > num3  && num1 > num4 && num1 > num5)
        printf("Leftmost");
    else if(num3 > num1 && num3 > num2 && num3 > num4 && num3 > num5)
        printf("Middle");
    else if(num5 > num1 && num5 > num2 && num5 > num3 && num5 > num4)
        printf("Rightmost");
    else
        printf("Unknown");
}
```