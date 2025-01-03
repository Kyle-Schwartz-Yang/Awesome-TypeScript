# TypeScript перегрузка функции (function overloading)

> TypeScript позволяет определять разные сигнатуры для функции, чтобы обрабатывать различные входные данные, сохраняя при этом одну реализацию

## Сигнатура функции — это ?

> Сигнатура функции — это описание того, как функцию можно вызывать. что Она определяет:

- Имя функции
- Тип и количество аргументов, которые функция принимает
- Тип возвращаемого значения

```ts
function print(value: string): void; // Сигнатура для строки
function print(value: number): void; // Сигнатура для числа

// Реализация с объединённой логикой
function print(value: string | number): void {
  if (typeof value === "string") {
    console.log(`Строка: ${value}`);
  } else {
    console.log(`Число: ${value}`);
  }
}
```

### Зачем нужны сигнатуры?

- **Для ясности и безопасности:** Сигнатуры помогают TypeScript точно знать, что ожидается на входе и что функция возвращает.
- **Для перегрузки функций:** Сигнатуры позволяют создавать несколько версий одной функции для разных типов данных, что делает код более гибким.

## Правила перезагрузки ?

- `Функция перезагрузки` могут иметь другие именна аргументов от основной.
- `Функция перезагрузки` не может иметь другие типы анотации в отличие от основной.
- `Функция перезагрузки` не влияет на скорость и бытует мнение что избыточно
