Пример:
```c
int a[10];
    
for (int i = 0; i < 10; i++) {
    scanf("%d", &a[i]);
}

for (int i = 0; i < 10; i++) {
    if (a[i] % 2 == 0) {
        a[i] /= 2;
    } else {
        a[i] *= 2;
    }
}

for (int i = 0; i < 10; i++) {
    printf("%d ", a[i]);
}
```