# Operator Non-Null

> Это возможность очень редкая, но мы ее все равно рассмотрим .


### Как использовать ?

> Операор используется когда мы на 100% знаем что сущность существует. 


1. Важно понимать что используя `Non-Null` мы отключаем typescript предупреждения для сущность и если поступать бездумно 
  то получим ошибку в момента запуска кода (runtime)
2. Использовать нужно только понимая что делаешь...


```Typescript
    function printLength(s: string | null): void {
    // Используем non-null assertion (!) оператор, чтобы указать, что s не null
    console.log(s!.length);
  }

  const maybeString: string | null = 'Hello';
  printLength(maybeString);  // Работает нормально, компилятор не выдаёт ошибку
```