# Лабораторная работа №2. Основы работы с массивами, функциями и объектами в JavaScript

## Цель работы

Изучить основы работы с массивами и функциями в JavaScript, применяя их для обработки и анализа транзакций.

## Примечание

Задания, помеченные `[extra]`, выполняются студентом дополнительно для получения более высокой оценки.

## Условие

Создайте консольное приложение для анализа транзакций.

### Шаг 1. Создание массива транзакций

1. Создайте файл `main.js` для размещения вашего кода.
2. Создайте массив объектов с транзакциями. Каждая транзакция должна содержать следующие свойства:

   - `transaction_id` - уникальный идентификатор транзакции.
   - `transaction_date` - дата транзакции.
   - `transaction_amount` - сумма транзакции.
   - `transaction_type` - тип транзакции (приход или расход).
   - `transaction_description` - описание транзакции.
   - `merchant_name` - название магазина или сервиса.
   - `card_type` - тип карты (кредитная или дебетовая).

   Примеры транзакций: [Link](files/transations.js). Можете использовать их для тестирования.

### Шаг 2. Реализация функций для анализа транзакций

Реализуйте следующие функции для анализа транзакций.

1. `getUniqueTransactionTypes(transactions)`
   - Возвращает массив уникальных типов транзакций.
   - Используйте `Set()` для выполнения задания.
2. `calculateTotalAmount(transactions)` – Вычисляет сумму всех транзакций.
3. `calculateTotalAmountByDate(transactions, year, month, day)` _[extra]_
   - Вычисляет общую сумму транзакций за указанный год, месяц и день.
   - Параметры year, month и day являются необязательными.
   - В случае отсутствия одного из параметров, метод производит расчет по остальным.
4. `getTransactionByType(transactions, type)` - Возвращает транзакции указанного типа (`debit` или `credit`).
5. `getTransactionsInDateRange(transactions, startDate, endDate)` – Возвращает массив транзакций, проведенных в указанном диапазоне дат от `startDate` до `endDate`.
6. `getTransactionsByMerchant(transactions, merchantName)` – Возвращает массив транзакций, совершенных с указанным `merchantName`.
7. `calculateAverageTransactionAmount(transactions)` – Возвращает среднее значение транзакций.
8. `getTransactionsByAmountRange(transactions, minAmount, maxAmount)` – Возвращает массив транзакций с суммой в заданном диапазоне от `minAmount` до `maxAmount`.
9. `calculateTotalDebitAmount(transactions)` – Вычисляет общую сумму дебетовых транзакций.
10. `findMostTransactionsMonth(transactions)` – Возвращает месяц, в котором было больше всего транзакций.
11. `findMostDebitTransactionMonth(transactions)` – Возвращает месяц, в котором было больше дебетовых транзакций.
12. `mostTransactionTypes(transactions)`
    - Возвращает каких транзакций больше всего.
    - Возвращает `debit`, если дебетовых.
    - Возвращает `credit`, если кредитовых.
    - Возвращает `equal`, если количество равно.
13. `getTransactionsBeforeDate(transactions, date)` – Возвращает массив транзакций, совершенных до указанной даты.
14. `findTransactionById(transactions, id)` – Возвращает транзакцию по ее уникальному идентификатору (`id`).
15. `mapTransactionDescriptions(transactions)` – Возвращает новый массив, содержащий только описания транзакций.

### Шаг 3. Тестирование функций

1. Создайте массив транзакций и протестируйте все функции.
2. Выведите результаты в консоль.
3. Проверьте работу функций на различных наборах данных.
4. Проверьте работу функций на пустом массиве транзакций _[extra]_.
5. Проверьте работу функций на массиве транзакций с одной транзакцией _[extra]_.

## Документирование кода

Код должен быть корректно задокументирован, используя стандарт `JSDoc`. Каждая функция и метод должны быть описаны с указанием их входных параметров, выходных данных и описанием функционала. Комментарии должны быть понятными, четкими и информативными, чтобы обеспечить понимание работы кода другим разработчикам.

## Контрольные вопросы

1. Какие методы массивов можно использовать для обработки объектов в JavaScript?
2. Как сравнивать даты в строковом формате в JavaScript?
3. В чем разница между `map()`, `filter()` и `reduce()` при работе с массивами объектов?
