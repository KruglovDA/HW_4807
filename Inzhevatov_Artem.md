#  <center><u>Руководство по Git</u></center>
## <u>Основные команды</u>
### Проверка репозитория
* <font color="yellow"> git --version</font> - показывает установленную версию Git.
* <font color="yellow"> git status</font> - отображает состояние рабочего каталога и раздела проиндексированных файлов. С ее помощью можно проверить индексацию изменений и увидеть файлы, которые не отслеживаются Git. Информация об истории коммитов проекта не отображается при выводе данных о состоянии.
* <font color="yellow"> git log</font> - отображает отправленные снимки состояния и позволяет просматривать и фильтровать историю проекта, а также проводить поиск по ней.
* <font color="yellow">git log</font> <font color="orange"> --graph --decorate --oneline</font> - Здесь содержится несколько полезных параметров: флаг<font color="orange"> --graph </font>создает основанную на тексте диаграмму коммитов в левой части области сообщений коммитов; флаг<font color="orange"> --decorate</font> добавляет отображаемые имена веток или теги коммитов; флаг<font color="orange"> --oneline</font> записывает информацию о коммите в одну строку, что позволяет без труда просматривать множество коммитов сразу.
* <font color="yellow">.gitignore</font> - позволяет игнорировать файлы поместив пути к ним в .gitignore

### Настройки репозитория
* <font color="yellow"> git init </font> - инициализирует локальный репозеторий.Команду выполняют только один раз для первоначальной настройки нового репозитория. Выполнение команды приведет к созданию нового подкаталога .git в вашем рабочем каталоге. Кроме того, будет создана новая главная ветка.
* <font color="yellow"> git clone</font> <font color="orange">repo url</font> - выполняют для создания копии (клонирования) удаленного репозитория. 

* Переключение между версиями -<font color="yellow
"> git checkout</font>  <font color="yellow">номер коммита</font>

* Вернуться обратно к тому коммиту в котором работали - <font color="yellow
">git checkout master</font>
>  <font color="orange">*Нажатие клавиши </font> <font color="yellow">"Q"</font> <font color="orange"> возвращает в исходное окно терминала.*</font>

* Показывает разницу между текущим файломи сохранённым -  <font color="yellow
">git diff</font>
* <font color="yellow">git remote</font> - просмотр списка удалённых репозиториев.
* <font color="yellow">git fetch</font> - загрузка изменений из удалённого репозитория без слияния с локальной веткой.
### Сохранение изменений
*  <font color="yellow">  git add</font> <font color="orange">Название файла</font>.<font color="yellow">Расширение файла</font> - добавляет содержимое рабочего каталога в индекс(staging area) для последующего коммита. Команда<font color ="yellow"> git add --all</font> добавляет все измененные и неотслеживаемые файлы в репозиторий и обновляет дерево изменений репозитория.
* <font color="yellow">git reset </font> - для отмены коммита или проиндексированного снимка состояния.
* <font color="yellow">git push</font> - используется для отправки подтвержденных изменений в удаленные репозитории для совместной работы, чтобы к набору сохраненных изменений могли получить доступ другие участники команды.
* <font color ="yellow">git commit -m </font><font color="orange">"Teкст сообщения"</font>
 Команда берёт все данные, добавленные в индекс с помощью <font color="yellow
">git add</font>, и сохраняет их
слепок во внутренней базе данных, а затем сдвигает указатель текущей ветки на этот слепок. 
### Ветки
* <font color ="yellow">git branch</font> <font color="orange"> "имя ветки"</font> - создание новой ветки.
* <font color ="yellow">git branch</font> - просмотр списка веток.
* <font color ="yellow">git merge</font> <font color="orange"> "имя ветки"</font> - слияние веток. Присоединение идет к текущей ветке на которой вы находитесь.
* <font color ="yellow">git checkout  </font> <font color="orange"> номер коммита</font> or<font color="orange"> название ветки</font>  -  переключает между версиями и ветками.
* <font color ="yellow">git checkout</font> <font color="orange">-b название ветки</font> - позволяет создать новую ветку и тут же переместиться на нее.
* <font color ="yellow">git branch  </font> <font color="orange">-d "имя ветки"</font> - удаление ветки
* <font color ="yellow">git branch</font><font color ="orange"> -r  </font> - просмотр списка удалённых веток.
* <font color ="yellow">git branch</font><font color ="orange"> -a  </font> - просмотр списка всех локальных и удалённых веток.
* <font color ="yellow">git branch</font><font color ="orange"> --track <branch_name> <remote_branch>  </font> - - создание локальной ветки, отслеживающей удалённую ветку.
* <font color ="yellow">git remote</font><font color ="orange"> add <remote_name> <remote_url>  </font> - добавление нового удалённого репозитория.
* <font color ="yellow">git remote</font><font color ="orange"> remove <remote_name>  </font>  - удаление удалённого репозитория.


## Выделение текста
### Списки
* Что бы добавить ненумерованные списки, необходимо пункты выделить звездочкой (<font color ="yellow">*</font>). Например, вот так:
* Элемент 1
* Элемент 2
* Элемент 3
* Что бы добавить нумерованные списки, необходимо пункты просто пронумеровать. Например вот так:
1. Элемент 1
2. Элемент 2
3. Элемент 3
## Форматирование текста
* Что бы создать заголовок выделите текст <font color ="yellow">#</font>. Заголовки могут быть разных уровней по аналогии с HTML(H1, H2 ..)

# <font color ="yellow">Заголовок</font>
* Чтобы выделить текст курсивом, необходимо обрамить его звёздочками (<font color ="yellow">*</font>). Например,
*вот так* <center>или</center>
* Чтобы выделить текст курсивом, необходимо обрамить его нижним подчеркиванием (<font color ="yellow">(_)</font>). Например,
_вот так_.
* Чтобы выделить текст полужирным, необходимо его обрамить двойными звёздочками<font color ="yellow">(**)</font>. 
Например, **вот так**.
### Решение проблем с SSH
* [Статья](https://umedman.gitbooks.io/-git-keys-/content/kodovie_frazi.html) о изменении кодовой фразы и автозапуск с SSH-agenta.

* [Cтатья](https://winitpro.ru/index.php/2022/12/22/nastrojka-ssh-vscode/) о
 настройке SSH подключений в Visual Studio Code.

### Дополнительная информация
* [Статья](https://gb.ru/posts/soveti-pro-git) про папки, репозитории и некоторые сложности при освоении контроля версий от Ильнара Шафигуллина.
* Дополнительный [курс](https://gb.ru/courses/1117) по Git.
* [скринкаст](https://vimeo.com/showcase/5616060?page=2)   от Ильи Кантора.










