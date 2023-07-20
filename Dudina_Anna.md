# Краткое руководство по Git.
## 1. Основные команды
* git init - инициализирует локальный репрозиторий 
## 2. Ветки
*git branch - выводит список веток
*git branch new_branch - создание новой ветки с именем new_branch
*git merge branch_name - выполняет слияние текущей ветки с веткой branch_name
## 3. Команды(продолжение)
*git status - Проверка статуса репозитория
*git commit -m "Ваш комментарий" - Внесение изменений однострочным сообщением или через редактор
* git show 1af17e73721dbe0c40011b82ed4bb1a7dbe3ce29 - Просмотр заданного коммита
* git diff - Просмотр изменений до коммита
* git remote add awesomeapp https://github.com/someurl.. - Добавление удалённого репозитория
* git revert HEAD - Откат последнего коммита

## Клонирование и создание репрозитория

### Создание репозитория в существующем каталоге
Если у вас уже есть проект в каталоге, который не находится под версионным контролем Git, то для начала нужно перейти в него.

для Windows:

$ cd C:/Users/user/my_project
а затем выполните команду:

$ git init
Эта команда создаёт в текущем каталоге новый подкаталог с именем .git, содержащий все необходимые файлы репозитория — структуру Git репозитория. На этом этапе ваш проект ещё не находится под версионным контролем.

Если вы хотите добавить под версионный контроль существующие файлы (в отличие от пустого каталога), вам стоит добавить их в индекс и осуществить первый коммит изменений. Добиться этого вы сможете запустив команду git add несколько раз, указав индексируемые файлы, а затем выполнив git commit:

$ git add *.c
$ git add LICENSE
$ git commit -m 'Initial project version'

### Клонирование существующего репозитория
Для получения копии существующего Git-репозитория, например, проекта, в который вы хотите внести свой вклад, необходимо использовать команду git clone. Если вы знакомы с другими системами контроля версий, такими как Subversion, то заметите, что команда называется «clone», а не «checkout». Это важное различие — вместо того, чтобы просто получить рабочую копию, Git получает копию практически всех данных, которые есть на сервере. При выполнении git clone с сервера забирается (pulled) каждая версия каждого файла из истории проекта. Фактически, если серверный диск выйдет из строя, вы можете использовать любой из клонов на любом из клиентов, для того, чтобы вернуть сервер в то состояние, в котором он находился в момент клонирования (вы можете потерять часть серверных хуков (server-side hooks) и т. п., но все данные, помещённые под версионный контроль, будут сохранены.

Клонирование репозитория осуществляется командой git clone <url>. Например, если вы хотите клонировать библиотеку libgit2, вы можете сделать это следующим образом:

$ git clone https://github.com/libgit2/libgit2
Эта команда создаёт каталог libgit2, инициализирует в нём подкаталог .git, скачивает все данные для этого репозитория и извлекает рабочую копию последней версии. Если вы перейдёте в только что созданный каталог libgit2, то увидите в нём файлы проекта, готовые для работы или использования. Для того, чтобы клонировать репозиторий в каталог с именем, отличающимся от libgit2, необходимо указать желаемое имя, как параметр командной строки:

$ git clone https://github.com/libgit2/libgit2 mylibgit
Эта команда делает всё то же самое, что и предыдущая, только результирующий каталог будет назван mylibgit.