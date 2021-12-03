# Ayala Parking Inc(from codeChum, modified)

```C
#include <stdio.h>

char getType() {
    char q;
    scanf("%c", & q);
    return q;
}

int getTime() {
    int q;
    scanf("%d", & q);
    return q;
}

int findHour(int timeIn, int timeOut) {
    int h;
    if ((timeOut % 100 < timeIn % 100)) {
        return ((timeOut / 100) - 1) - (timeIn / 100);
    }
    return (timeOut / 100) - (timeIn / 100);
}

int findMin(int timeIn, int timeOut) {
    int m;
    if ((timeOut % 100 < timeIn % 100)) {
        return ((timeOut % 100) + 60) - (timeIn % 100);
    }
    return (timeOut % 100) - (timeIn % 100);
}

float computeParking(char type, int hour, int min) {
    switch (type) {
    case 'M':
        if (hour > 3) {
            return (hour - 3) * 10.0;
        } else return 0.00;
        break;
case 'C':
        if (hour > 3) {
            return ((hour - 3) * 10.0) + (30.00);
        } else return 30.00;
        break;
    case 'T':
        if (hour > 3) {
            return ((hour - 3) * 25.0) + (50.00);
        } else return 50.00;
        return 0;
    }
}

void display(float pay, int hour, int min) {
    printf("Payment: %.2f\n", pay);
    printf("Hours: %d\n", hour);
    printf("Minutes: %d\n", min);

    return;
}
```

# Mysterious Blue (from codeChum, modified)

```C
#include<stdio.h>

int getAge() {
    int age;
    scanf("%d", & age);
    return age;
}
void display(int age) {
    if (age < 18) {
        printf("minor");
    } else if (age >= 18 && age < 60) {
        printf("adult");
    } else {
        printf("senior");
    }
    return;
}
```

# Age Category(from codeChum, modified)

```C
#include<stdio.h>

int getAge() {
    int age;
    scanf("%d", & age);
    return age;
}
/*get age as input from the user*/

void display(int age) {
    if (age >= 0 && age <= 12) {
        printf("Child");
    } else if (age >= 13 && age <= 17) {
        printf("Teenager");
    } else if (age >= 18 && age <= 59) {
        printf("Adult");
    } else if (age >= 60) {
        printf("Senior Citizen");
    }
}

/*prints the following:
Child - 0 to 12 years old
Teenager - 13 to 17 years old
Adult - 18 to 59 years old
Senior Citizen - 60 years old and above
*/
```