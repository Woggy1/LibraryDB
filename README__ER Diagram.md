Сутності:

Книга (Book):

book_id (ключ)
title
ISBN
publication_year
...
Автор (Author):

author_id (ключ)
name
birthdate
...
Жанр (Genre):

genre_id (ключ)
name
...
Читач (Reader):

reader_id (ключ)
name
email
...
Видача (Loan):

loan_id (ключ)
book_id (зовнішній ключ, посилається на book_id у таблиці Book)
reader_id (зовнішній ключ, посилається на reader_id у таблиці Reader)
date_borrowed
date_returned
...
Взаємозв'язки:

Взаємозв'язок "Авторство" (Authorship) між таблицями Author та Book.

Один автор може мати багато книг.
Кожна книга може мати одного або багато авторів.
Взаємозв'язок "Належить до жанру" (Belongs To Genre) між таблицями Book та Genre.

Кожна книга може належати до одного жанру.
Кожен жанр може мати багато книг.
Взаємозв'язок "Видача" (Loan) між таблицями Book та Reader.

Кожна книга може мати багато видач.
Кожен читач може мати багато видач.
