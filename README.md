# Задача 1. Пакування товарів

 

Напиши функцію `isEnoughCapacity(products, containerSize)`, яка обчислює, чи помістяться всі товари в контейнер при пакуванні.

### Параметри:
- `products` — об’єкт, у якому ключі містять назви товарів, а їхні значення — кількість цих товарів.  
  Наприклад: `{ apples: 2, grapes: 4 }`
- `containerSize` — число, максимальна кількість одиниць товарів, яку може вмістити контейнер.

### Опис:
Функція має повернути `true`, якщо загальна кількість товарів менша або дорівнює `containerSize`, і `false`, якщо більша.

### Приклади використання:
```javascript
console.log(
  isEnoughCapacity({ apples: 2, grapes: 3, carrots: 1 }, 8)
); // true

console.log(
  isEnoughCapacity({ apples: 4, grapes: 6, lime: 16 }, 12)
); // false

console.log(
  isEnoughCapacity({ apples: 1, lime: 5, tomatoes: 3 }, 14)
); // true

console.log(
  isEnoughCapacity({ apples: 18, potatoes: 5, oranges: 2 }, 7)
); // false
```

Залиш цей код для перевірки ментором.

### Ментор перевірятиме:
- Оголошена функція `isEnoughCapacity(products, containerSize)`
- Правильність результатів усіх тестів

---

# Задача 2. Розрахунок калорій

 

Напиши функцію `calcAverageCalories(days)`, яка повертає середньодобову кількість калорій, які спортсмен споживав протягом тижня.

### Параметри:
- `days` — масив об’єктів. Кожен об’єкт має властивості:
  - `day` — назва дня
  - `calories` — кількість калорій, спожитих у цей день

### Приклади використання:
```javascript
console.log(
  calcAverageCalories([
    { day: "monday", calories: 3010 },
    { day: "tuesday", calories: 3200 },
    { day: "wednesday", calories: 3120 },
    { day: "thursday", calories: 2900 },
    { day: "friday", calories: 3450 },
    { day: "saturday", calories: 3280 },
    { day: "sunday", calories: 3300 }
  ])
); // 3180

console.log(
  calcAverageCalories([
    { day: "monday", calories: 2040 },
    { day: "tuesday", calories: 2270 },
    { day: "wednesday", calories: 2420 },
    { day: "thursday", calories: 1900 },
    { day: "friday", calories: 2370 },
    { day: "saturday", calories: 2280 },
    { day: "sunday", calories: 2610 }
  ])
); // 2270

console.log(
  calcAverageCalories([])
); // 0
```

 
# Задача 3. Профіль гравця

**ВИКОНУЙ ЦЕ ЗАВДАННЯ У ФАЙЛІ `task-3.js`**

Об’єкт `profile` описує профіль користувача на ігровій платформі.

```javascript
const profile = {
  username: "Jacob",
  playTime: 300,
};
```

### Необхідно:
Доповнити об’єкт методами:

- `changeUsername(newName)` — приймає нове ім’я (рядок) і змінює `username`.
- `updatePlayTime(hours)` — приймає число і додає до `playTime`.
- `getInfo()` — повертає рядок у форматі:
  ```
  <Username> has <amount> active hours!
  ```

 
