Пример:
```c
int a[5];

printf("Введите 5 элементов массива: ");
for (int i = 0; i < 5; i++) {
    scanf("%d", &a[i]);
}

for (int i = 0; i < 5; i++) {
    if (a[i] % 2 == 0) {
        a[i] /= 2;
    } else {
        a[i] *= 2;
    }
}

printf("Измененный массив: ");
for (int i = 0; i < 5; i++) {
    printf("%d ", a[i]);
}
```
Индекс первого вхождения элемента в массиве
```c
int a[5];

printf("Введите 5 элементов массива: ");
for (int i = 0; i < 5; i++) {
    scanf("%d", &a[i]);
}

int value;
printf("Введите искомый элемент: ");
scanf("%d", &value);

int index = -1;
for (int i = 0; i < 5; i++) {
    if (a[i] == value) {
        index = i;
    }
}

if (index == -1) {
    printf("Элемент '%d' не найден", value);
} else {
    printf("Индекс элемента '%d' в массиве равен '%d'", value, index);
}
```
Задание 1  
Что выведет программа если ввести:  
a)  
```
1 2 3 4 5
3
```
b) 
```
1 2 3 4 5
6
```
