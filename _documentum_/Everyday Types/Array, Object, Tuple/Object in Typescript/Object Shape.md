

# Продвинутый Type и пересечение типов ( Intersection -- используя оператор (&) )
 
> Можно воспользоваться алясом для создание аннотации объекта или создать альас для функции


### Использование aliases для объекта 

- Можна використовувати [[Type Aliases]]  для створення анотацій об'єктів. 
- Однак, зазвичай для цього частіше використовують [[Type Interfeces]] оскільки вони надають додаткову гнучкість і можливості.

```typescript
/* Создание aliases */
  type Person = {
    name: string;
    age: number;
    isEmployed: boolean;
  }

/* Теперь можно использовать aliases где угодно. */
  const person: Person = {
    name: 'John',
    age: 30,
    isEmployed: true
  };
```

