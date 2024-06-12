### Клиент-серверное приложение для общения пользователей друг с другом (чат)

Проект на языке Java с использованием библиотеки Swing для создания графического интерфейса

Выполнено разделение логики работы сервера (класс Server) и графической части сервера (класс ServerGUI).

Методы работы абстрактного сервера выделены в интерфейс ServerView, класс Server реализует данные методы.
Графический класс принимает на вход в свой конструктор абстракцию (любой класс, реализующий интерфейс ServerView) и работает с методами данной абстракции.

Таким образом, графический класс ничего не знает про класс Server и не зависит от него, а класс Server ничего не знает про графику и библиотеку Swing. Классы ничего не знают друг о друге и не зависят друг от друга, зависимость построена на абстракции, т.е. с помощью интерфейса реализован пятый принцип SOLID - принцип инверсии зависимостей.

Лог чата записывается в текстовый файл и загружается при запуске сервера
###
Для начала работы необходимо запустить файл приложения Main

#### Скриншот:

![Screenshot15.png](https://raw.githubusercontent.com/romanyukalexandr84/Images/main/Screenshot15.png)
