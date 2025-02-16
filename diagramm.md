Мы выделяем четыре таблицы:

- **customers**: хранит информацию о клиентах
- **transactions**: хранит данные о транзакциях
- **products**: хранит сведения о товарах/услугах
- **transaction_items**: связка “многие ко многим” между `transactions` и `products`


customers (1) 
   └─ (M) transactions (1)
           └─ (M) transaction_items (M) ─ (1) products
