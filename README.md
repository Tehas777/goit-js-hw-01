# goit-js-hw-01

Формат здачі

Здай на платформі LMS два посилання:

на репозиторій з кодом;
на живу сторінку на GitHub Pages.


Задача 1. Замовлення дроїдів

Виконуй це завдання у файлі task-1.js
Станція з продажу ремонтних дроїдів готова до запуску — залишилося написати програмне забезпечення для відділу продажів.



Оголоси функцію makeTransaction, яка очікує два параметри:

quantity — число, кількість замовлених дроїдів
pricePerDroid — число, вартість одного дроїда


Значення параметрів задаються під час виклику. Функція повертає рядок:

You ordered <quantity> droids worth <totalPrice> credits!



Де:

<quantity> — кількість замовлених дроїдів
<totalPrice> — загальна вартість замовлення (вартість усіх замовлених дроїдів)


Встав код нижче після оголошення функції для перевірки. Залиш його для перевірки ментором.

console.log(makeTransaction(5, 3000)); // "You ordered 5 droids worth 15000 credits!"
console.log(makeTransaction(3, 1000)); // "You ordered 3 droids worth 3000 credits!"
console.log(makeTransaction(10, 500)); // "You ordered 10 droids worth 5000 credits!"



Вимоги

Оголошено функцію makeTransaction(quantity, pricePerDroid).
Виклик makeTransaction(5, 3000) повертає "You ordered 5 droids worth 15000 credits!".
Виклик makeTransaction(3, 1000) повертає "You ordered 3 droids worth 3000 credits!".
Виклик makeTransaction(10, 500) повертає "You ordered 10 droids worth 5000 credits!".
Виклик з будь-якими валідними аргументами повертає правильне значення.
Результати всіх викликів виведено в консоль.


Задача 2. Доставка товару

Виконуй це завдання у файлі task-2.js


Оголоси функцію getShippingMessage, яка очікує три параметри:

country — рядок, країна доставки
price — число, вартість товару
deliveryFee — число, вартість доставки


Значення параметрів задаються під час виклику. Функція повертає рядок:

Shipping to <country> will cost <totalPrice> credits



Де:

<country> — країна доставки
<totalPrice> — загальна вартість, що включає вартість товару і доставки


Встав код нижче після оголошення функції для перевірки. Залиш його для перевірки ментором.

console.log(getShippingMessage("Australia", 120, 50)); // "Shipping to Australia will cost 170 credits"
console.log(getShippingMessage("Germany", 80, 20)); // "Shipping to Germany will cost 100 credits"
console.log(getShippingMessage("Sweden", 100, 20)); // "Shipping to Sweden will cost 120 credits"



Вимоги

Оголошено функцію getShippingMessage(country, price, deliveryFee).
Виклик getShippingMessage("Australia", 120, 50) повертає "Shipping to Australia will cost 170 credits".
Виклик getShippingMessage("Germany", 80, 20) повертає "Shipping to Germany will cost 100 credits".
Виклик getShippingMessage("Sweden", 100, 20) повертає "Shipping to Sweden will cost 120 credits".
Виклик з будь-якими валідними аргументами повертає правильне значення.
Результати всіх викликів виведено в консоль.


Задача 3. Ширина елемента

Виконуй це завдання у файлі task-3.js


Оголоси функцію getElementWidth, яка очікує три параметри:

content — число, ширина контенту
padding — число, горизонтальний паддінг для кожної зі сторін
border — число, товщина бордера для кожної зі сторін


Значення параметрів — числа, цілі або дробові. Функція повертає число — загальну ширину елемента за формулою:

загальна ширина = content + padding * 2 + border * 2



Встав код нижче після оголошення функції для перевірки. Залиш його для перевірки ментором.

console.log(getElementWidth(50, 8, 4)); // 74
console.log(getElementWidth(60, 12, 8.5)); // 101
console.log(getElementWidth(200, 0, 0)); // 200



Вимоги

Оголошено функцію getElementWidth(content, padding, border).
Виклик getElementWidth(50, 8, 4) повертає число 74.
Виклик getElementWidth(60, 12, 8.5) повертає число 101.
Виклик getElementWidth(200, 0, 0) повертає число 200.
Функція повертає число, а не рядок.
Виклик з будь-якими валідними аргументами повертає правильне значення.
