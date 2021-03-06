## Тестовые задания для Python

### Задача 1: Что может быть проще SQL?

Вам дана таблица в postgres, которая представляет из себя список сотрудников с их зарплатами и отделами.
Необходимо написать запрос, который будет выбирать человека с максимальной зарплатой из каждого отдела. В качестве тестовых данных можете использовать [дамп таблицы](employee.sql), пример схемы:
```
postgres=# \d employee
            Table "public.employee"
   Column   |         Type          | Modifiers
------------+-----------------------+-----------
 id         | integer               | not null
 name       | character varying(30) |
 department | character varying(30) |
 salary     | integer               |
Indexes:
    "employee_pkey" PRIMARY KEY, btree (id)
```


### Задача 2: Smashing Wallpaper Downloader

Есть прекрасный сайт Smashing Magazine, который каждый месяц выкладывает отличные обои для десктопа. Заходить каждый месяц и проверять, что там нового дело не благородное, поэтому давайте попробуем автоматизировать эту задачу.
Требуется написать cli утилиту, которая будет качать все обои в требуемом разрешение за указанный месяц-год в текущую директорию пользователя. Вот [тут](https://www.smashingmagazine.com/tag/wallpapers/) находятся все обои, а [здесь](https://www.smashingmagazine.com/2017/04/desktop-wallpaper-calendars-may-2017/) находятся обои за май 2017.

Условия:
* Python 3.5+
* Любые сторонние библиотеки
* PEP8
* Если останется время, то можете покрыть её тестами с помощью py.test (:
