# Материалы по курсу "Основы языка и платформы Java для анализа данных"

## Тема 1. Основы языка
- [Презентация](https://disk.yandex.ru/i/59AdRUKocrkXgg)
## Тема 2. Типы данных
- [Примеры кода](basics/src/main/java/ru/msu/vmk/Main.java)
- [Презентация](https://disk.yandex.ru/i/EZSzwSpcYPa0rw)

## Задание 1:
Дан следующий код, необходимо реализовать метод split.
```java
public class NumberSample {

    public static void main(String[] args) {
      // вызов split - проверка работы
    }

    public static BigDecimal[] split(BigDecimal amount, int n) {
        // разделить amount на n частей
        // если остается остаток, прибавить его к первому числу
        return null;
    }
}
```
- [Место для реализации](basics/src/main/java/ru/msu/vmk/NumberSample.java)
- [Тесты для проверки](basics/src/test/java/NumberSampleTests.java)

## Тема 3. Объектно ориентированное программирование
- [Примеры кода](object-oriented-programming/src/main/java/ru/msu/vmk)
- [Презентация](https://disk.yandex.ru/i/FvM8OJUHVnF0Gw)

## Задание 2:
По примеру класса [Money](object-oriented-programming/src/main/java/ru/msu/vmk/Money.java) реализовать класс [Quantity](object-oriented-programming/src/main/java/ru/msu/vmk/Quantity.java):
- с поддержкой единиц измерения
- арифметических операций: add, subtract, multiply, divide
- реализовать операцию деления на N равных частей с добавлением остатка к первому значению (см. предыдущее задание)
- для проверки работы реализовать функцию main() или Unit-test по примеру
- [Место для реализации](object-oriented-programming/src/main/java/ru/msu/vmk/Quantity.java)
- [Тесты для проверки](object-oriented-programming/src/test/java/QuantityTest.java)

## Тема 4. Коллекции
- [Примеры кода](collections/src/main/java/ru/msu/vmk)
- [Презентация](https://disk.yandex.ru/i/ZhM3kx6VsYPqxg)

## Задание 3:
- Реализовать интерфейс [Library](collections/src/main/java/ru/msu/vmk/Library.java) в [LibraryImpl](collections/src/main/java/ru/msu/vmk/LibraryImpl.java) с использованием Java Collections
- Для проверки работы реализовать [Unit-test](collections/src/test/java/LibraryImplTest.java)
```java
/* Институтская библиотека */
public interface Library {
    /* Регистрация новой книги */
    void addNewBook(Book book);
    /* Студент берет книгу */
    void borrowBook(Book book, String student);
    /* Студент возвращает книгу */
    void returnBook(Book book, String student);
    /* Получить список свободных книг */
    List<Book> findAvailableBooks();
}
```

## Тема 5. Maven
- [Примеры кода](maven/src/main/java/ru/msu/vmk)
- [Презентация](https://disk.yandex.ru/d/AD0DLwOAK_2jjA)

## Тема 6. Ввод-вывод в Java
- [Примеры кода](input-output/src/main/java/ru/msu/vmk)
- [Презентация](https://disk.yandex.ru/i/bdFL3BQY8mcIdw)

## Порядок сдачи заданий
1. Сделать fork этого репозитория к себе в аккаунт
![img/img.png](img/img.png)
2. Клонировать репозиторий(именно из своего аккаунта) на свою машину(инструкция по интеграция гита с intellij размещена ниже) ![img/img_1.png](img/img_1.png)
3. Выполнить задание(ссылки и постанока задачи размещены выше)
4. Сделать коммит и пуш ![img/img_2.png](img/img_2.png)
5. Создать pull request в основной репозиторий курса(https://github.com/sh-vasily/java-basics)
![img/img_3.png](img/img_3.png)
При этом необходимо, чтобы тесты для задания, которое вы сдаете успешно прошли в github actions.
![img/img_4.png](img/img_4.png)
К примеру, если это задание по коллекциям, рядом с collections должен быть зеленый кружок.

## Софт
- https://git-scm.com/downloads
- https://www.jetbrains.com/idea/
- https://www.java.com/ru/download/
- https://www.oracle.com/cis/java/technologies/downloads/
- https://maven.apache.org/

## Книги по Java
- Брюс Эккель - Философия Java
- Head First Java, Кэти Сиерра и Берт Бейтс
- Кей Хорстманн «Java. Библиотека профессионала» (Core Java)

## Курсы по Java
- [Разработка на java](https://www.youtube.com/playlist?list=PLrCZzMib1e9qUdn_LEm96Oee3RVb9Qmr_) 

## Курсы по git
- https://javarush.com/groups/posts/2818-podruzhim-git-s-intellij-idea - Интеграция github и intellij. Ёмко и кратко о том, что может понадобится. Рекомендую
- https://www.youtube.com/watch?v=EeARyFrZsnU - короткий ролик про git, дает концептуальное понимание
- https://habr.com/ru/articles/541258/ - Git для новичков
- https://githowto.com/ru - гайд по гиту с удобным визардом
- https://git-scm.com/book/ru/v2/ - книга по гиту, не нужно читать всё, достаточно смотреть необходимую информацию

## Курсы по алгоритмам 
- https://education.yandex.ru/handbook/algorithms