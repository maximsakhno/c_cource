# Строки

#### Пример 1
Операции с одной строкой

```c
#include <stdio.h>
#include <string.h>

int main(void) {
    char string[128];
    
    scanf("%s", string);
    printf("string = %s\n", string);
    
    int string_length = strlen(string);
    printf("string_length = %d\n", string_length);
    
    if (string_length > 0) {
        char first_symbol = string[0];
        printf("first_symbol = %c\n", first_symbol);

        string[0] = 'a';
        printf("string = %s\n", string);
    }

    string[0] = '\0';
    printf("string = %s\n", string);

    return 0;
}
```

#### Задание 1
Создать программу, выводяющую каждый символ строки на новой строке.

#### Задание 2
Создать программу, проверяющую, является ли строка палиндромом.

#### Пример 2
Сравнение строк

```c
#include <stdio.h>
#include <string.h>

int main(void) {
    char string1[128] = "hello world";
    char string2[128] = "world";

    printf("string1 = %s\n", string1);
    printf("string2 = %s\n", string2);

    int compare_result = strcmp(string1, string2);
    if (compare_result > 0) {
        printf("string1 > string2\n");
    } else if (compare_result < 0) {
        printf("string1 < string2\n");
    } else {
        printf("string1 = string2\n");
    }

    return 0;
}
```

#### Задание 3
Создать программу, считывающую логин и пароль и проверяющую их.

#### Задания на acmp.ru
* [Номера автобусов](https://acmp.ru/index.asp?main=task&id_task=691)
* [Сжатие бинарных последовательностей](https://acmp.ru/index.asp?main=task&id_task=950)
* [Стрелки](https://acmp.ru/index.asp?main=task&id_task=44)
* [Нумеролог](https://acmp.ru/index.asp?main=task&id_task=95)
