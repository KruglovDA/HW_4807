# Руководство по Git
### Контроль версий — практика, которая позволяет отслеживать изменения исходного кода и управлять ими.
Необходим, чтобы:
* хранить разные версии проекта;
* возвращаться к разным версиям проекта.

## Основные команды
* **git --version** - проверка текущей установленной
версии пограммы;
* **git init** - инициализирует локальный репозиторий;
* **git status** - показывает текущее состояние гита, есть ли изменения, которые нужно сохранить;
* **git add <имя файла.расширение>** - добавляет содержимое рабочего каталога в индекс для последующего коммита (эта команда дается после добавления
файлов);
* **git commit -m "комментарий"** - зафиксировать или сохранить, эта команда берёт все данные, добавленные в индекс с помощью git add, и сохраняет их
слепок во внутренней базе данных, а затем сдвигает указатель текущей ветки на этот слепок;
* **git log** - журнал изменений *(нажатие клавиши ‘Q’ возвращает в исходное окно терминала)*;
* **git checkout** - переключение между версиями;
* **git diff** - показывает разницу между текущим файлом и сохранённым.

## Работа с ветками
* **git branch <имя ветки>** - создание ветки;
* **git branch** - вывод на экран ветки, где находимся;
* **git checkout <имя ветки>** - переключение на другую ветку;
* **git merge <имя ветки>** - слияние ветки с *текущей*;
* **git branch -d <имя ветки>** - удаление ветки;
* **git log --graph** - визуализация в виде дерева.
### Конфликт изменений
При работе в двух ветках одновременно может возникнуть ситуация, когда в одной и другой ветке мы по-разному изменили блок текста. Если затем мы попробуем слить эти ветки, Git сообщит о конфликте и предложит выбрать,
какие же изменения записать.

## Работа с удаленными репозиториями
* **git clone** - загружает все изменения и пытается слить все ветки на локальном компьютере и в удаленном репозитории;
* **git pull** -  позволяет скачать все из текущего репозитория и автоматически сделать merge с нашей версией;
* **git push** - позволяет отправить нашу версию репозитория на внешний репозиторий;
* **pull request** - команда для предложения изменений, запрос на вливание изменений в репозиторий;
### *Как сделать pull request:*
1. Делаем ответвление репозитория **fork**
2. Делаем **git clone** версии репозитория СВОЕЙ
3. Создаем новую ветку и в нее вносим свои изменения
4. Фиксируем изменения **git commit**
5. Отправляем свою версию в свой GitHub
6. На сайте GitHub нажимаем кнопку **pull request**