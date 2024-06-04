# vk_contest_2

Хранения информации о пользователях и товарах - реляционная база данных. В частности PostgreSQL 
Хранение медиаконтента - файловая система; получение доступа к медиаконтенту через Nginx
Полнотекстовый поиск - Elasticsearch

Почему Реляционная бд:
- Имеется четкая структура и определенные связ; не требуется анализ связей
- Гарантия целостности данных. Манипуляции группой/категорией/подкатегорией
- С помощью языка запросов SQL легко манипулировать данными о продуктах и складах
- Удобно произвести шардирование по городам

Почему файловая система и Nginx:
- Возможность кеширования статических файлов
- Простая манипуляция статическими данными

Почему elasticsearech:
- Отсутствие транзакций и иных проверок, которые есть во всех базах. Что приведет к меньшему времени поиска по сравнению с использованием одной из СУБД для поиска

## Ссылки на схемы
- [Даталогическая модель](https://t.ly/g9Ybk) для PostgreSQL
- [UML схема системы](https://t.ly/PjYGP)
