# *Инструкция для работы с GIT* 
![](git_logo.png)

Git - консольное приложение для отслеживания изменений в файлах. В локальном репозитории хранятся файлы и история их изменения. Каждая точка сохранения - коммит с названием в виде хэш-кода. Позволяет возвращаться между сохранениями, оветвлять и сливать ветки состояния файла.

## Основные команды Git

* git init - инициализация локального репозитория
* git status - получить информацию о git, о его текущем состоянии
* git add - добавить файл или папку к следующему коммиту
* git commit -m "комментарий" - создание коммита
* git log - вывод на экран истории всех коммитов с их хэш-кодом
* git checkout - переход от одного коммита к другому
* git checkout master - вернуться к актуальному состоянию и продолжить работу
* git diff - увидеть разницу между текущим файлом и закоммиченным файлом
* git clone - клонировать репозиторий в папку
* git mv - переместить или переименовать файл или директорию

[Git для новичков (часть 1)](https://habr.com/ru/articles/541258/)

[Документация](https://git.github.io/htmldocs/git.html)

>--git-dir=<path<path>>
>Set the path to the repository (".git" directory). This can also be controlled by setting the GIT_DIR environment variable. It can be an absolute path or relative path to current working directory.

### Ответвления версий файла в Git

Git позволяет создавать, удалять сливать ветки версии файла, а также переходить между ними

+ git branch <название ветки> – создать новую ветку
+ git branch - посмотреть перечень имеющихся веток
+ git log --graph - вывести историю коммитов и ответвлений с графическим представлением
+ git checkout <название ветки> – переход к другой ветке
+ git branch -d <название ветки> – удалить ветку
+ git merge <название ветки> – слияние текущей ветки с указанной

### Команды для работы с внешними репозиториями

+ git clone <url-адрес репозитория> <название папки для клона репозитория> – клонирование внешнего репозитория на  локальный ПК
+ git pull – получение изменений и слияние с локальной версией
+ git push – отправляет локальную версию репозитория на внешний