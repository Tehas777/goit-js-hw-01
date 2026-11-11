
# goit-js-hw-01

Домашнє завдання

## Що зробиш
Напишеш три невеликі функції, які приймають дані, обчислюють результат і повертають його.

## Підготовка
- Створи репозиторій `goit-js-hw-01` та склонуй його собі на комп'ютер.
- У папці `goit-js-hw-01` створи структуру проєкта, як показано на схемі нижче.

> Зверни увагу! Імена файлів і папок та їхня структура вкладеності мають відповідати схемі. Інакше робота не буде прийнята.

```text
goit-js-hw-01/
├── js/
│   ├── task-1.js
│   ├── task-2.js
│   └── task-3.js
├── .gitignore
├── .prettierrc
├── index.html
└── README.md
```

- Прочитай кожне завдання і виконай його у відповідному файлі.
- Переконайся, що код відформатований Prettier, а в консолі немає помилок і попереджень під час відкриття живої сторінки завдання.

## Формат здачі
Здай на платформі LMS два посилання:
- на репозиторій з кодом;
- на живу сторінку на GitHub Pages.

---

## Задача 1. Замовлення дроїдів
Виконуй це завдання у файлі `js/task-1.js`.  
Станція з продажу ремонтних дроїдів готова до запуску — залишилося написати програмне забезпечення для відділу продажів.

Оголоси функцію `makeTransaction`, яка очікує два параметри:
- `quantity` — число, кількість замовлених дроїдів
- `pricePerDroid` — число, вартість одного дроїда

Значення параметрів задаються під час виклику. Функція повертає рядок:
> `You ordered <quantity> droids worth <totalPrice> credits!`

Де:
- `<quantity>` — кількість замовлених дроїдів
- `<totalPrice>` — загальна вартість замовлення (вартість усіх замовлених дроїдів)

Встав код нижче після оголошення функції для перевірки. Залиш його для перевірки ментором.

```javascript
console.log(makeTransaction(5, 3000)); // "You ordered 5 droids worth 15000 credits!"
console.log(makeTransaction(3, 1000)); // "You ordered 3 droids worth 3000 credits!"
console.log(makeTransaction(10, 500)); // "You ordered 10 droids worth 5000 credits!"
```

### Вимоги
- Оголошено функцію `makeTransaction(quantity, pricePerDroid)`.
- Виклик `makeTransaction(5, 3000)` повертає `"You ordered 5 droids worth 15000 credits!"`.
- Виклик `makeTransaction(3, 1000)` повертає `"You ordered 3 droids worth 3000 credits!"`.
- Виклик `makeTransaction(10, 500)` повертає `"You ordered 10 droids worth 5000 credits!"`.
- Виклик з будь-якими валідними аргументами повертає правильне значення.
- Результати всіх викликів виведено в консоль.

---

## Задача 2. Доставка товару
Виконуй це завдання у файлі `js/task-2.js`.

Оголоси функцію `getShippingMessage`, яка очікує три параметри:
- `country` — рядок, країна доставки
- `price` — число, вартість товару
- `deliveryFee` — число, вартість доставки

Значення параметрів задаються під час виклику. Функція повертає рядок:
> `Shipping to <country> will cost <totalPrice> credits`

Де:
- `<country>` — країна доставки
- `<totalPrice>` — загальна вартість, що включає вартість товару і доставки

Встав код нижче після оголошення функції для перевірки. Залиш його для перевірки ментором.

```javascript
console.log(getShippingMessage("Australia", 120, 50)); // "Shipping to Australia will cost 170 credits"
console.log(getShippingMessage("Germany", 80, 20)); // "Shipping to Germany will cost 100 credits"
console.log(getShippingMessage("Sweden", 100, 20)); // "Shipping to Sweden will cost 120 credits"
```

### Вимоги
- Оголошено функцію `getShippingMessage(country, price, deliveryFee)`.
- Виклик `getShippingMessage("Australia", 120, 50)` повертає `"Shipping to Australia will cost 170 credits"`.
- Виклик `getShippingMessage("Germany", 80, 20)` повертає `"Shipping to Germany will cost 100 credits"`.
- Виклик `getShippingMessage("Sweden", 100, 20)` повертає `"Shipping to Sweden will cost 120 credits"`.
- Виклик з будь-якими валідними аргументами повертає правильне значення.
- Результати всіх викликів виведено в консоль.

---

## Задача 3. Ширина елемента
Виконуй це завдання у файлі `js/task-3.js`.

Оголоси функцію `getElementWidth`, яка очікує три параметри:
- `content` — число, ширина контенту
- `padding` — число, горизонтальний паддінг для кожної зі сторін
- `border` — число, товщина бордера для кожної зі сторін

Значення параметрів — числа, цілі або дробові. Функція повертає число — загальну ширину елемента за формулою:
> `загальна ширина = content + padding * 2 + border * 2`

Встав код нижче після оголошення функції для перевірки. Залиш його для перевірки ментором.

```javascript
console.log(getElementWidth(50, 8, 4)); // 74
console.log(getElementWidth(60, 12, 8.5)); // 101
console.log(getElementWidth(200, 0, 0)); // 200
```

### Вимоги
- Оголошено функцію `getElementWidth(content, padding, border)`.
- Виклик `getElementWidth(50, 8, 4)` повертає число `74`.
- Виклик `getElementWidth(60, 12, 8.5)` повертає число `101`.
- Виклик `getElementWidth(200, 0, 0)` повертає число `200`.
- Функція повертає число, а не рядок.
- Виклик з будь-якими валідними аргументами повертає правильне значення.
