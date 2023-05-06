front <----> back <-----> DB (PostgreSQL) 

Technologies: 
- boot
- web
- security
- thyneleaf
- data jpa + postgresql
- additional: 
	- flyway
	- lombok

Features:
- Аутентификация и регистрация пользователей.
- Защита веб-приложения. 
- Просмотр товаров.
- добавление товаров в корзину.
- Формирование заказов. 
- Оплата (PayPal).
- Фильтрация/сортировка товаров.
- Управление корзиной.
- Валидация вводимых данных.
- Оповещения по emall.
- Навигация.


Entytles:
1. Product
	- id
	- title
	- price
	- categories
	- nds, sales (optional)
	- archive


2. User
	- id
	- username
	- emall
	- password
	- role
	- address (optional)
	- phone
	
3. Role
	- USER
	- GUEST
	- ADMIN
	- MANAGER

4. Order

	-td
	- created date
	- Last change date
	- completed date
	- adress 
	- user
	- status ( NEW, CANCEL, PAID, CLOSED)
	- details (product, price, amount, comment)

5. Category
	- id
	- title

6. Bucket
	- id
	- user
	- details (price, amount)
