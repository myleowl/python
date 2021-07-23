# python

В процессе работы мы часто пользуемся разными источниками данных, и
это не всегда готовые базы данных. Иногда данные нужно добывать с помощью
API.

Допустим, нам интересно, на каких позициях наше мобильное приложение или
приложение конкурентов. Чаще всего приложения ищутся по словам в их названии (не
обязательно на первом месте). Для того, чтобы узнать конкретную позицию по
конкретным словам, можно воспользоваться API iTunes.

Пусть id - appleid приложения, которое мы хотим исследовать (например, 860011430). У
этого приложения есть название из N слов (в данном случае "Ghost Lens AR Fun Movie
Maker"). Нужно написать python-скрипт, который принимает на вход id и заносит в sqlite3
базу данных itunes.db в таблицу itunes (id, word, pos, date) N строк; в каждой строке
написано id приложения, запрашиваемое слово из названия, позиция приложения id в
выдаче по этому слову и дата запуска скрипта
