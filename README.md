# LR6
##Лабораторная работа №6

### Цель лабораторной работы: 
Изучение базовых возможностей системы управления версиями, опыт работы с Git Api, опыт работы с локальным и
удаленным репозиторием. 

### Порядок выполнения лабораторной работы

1. Создать аккаунт на сайте GitHub
2. Сделать копию в личное хранилище из https://github.com/Kurtyanik/LR6/ (Fork).
3. Установить Git (https://git-scm.com/)
4. После установки настроить клиент git, введя имя пользователя и email.
Настройка производится с использованием команд `git config user.name` и `git config user.email`
![-](https://github.com/shadapovatsyrena/LR6/blob/master/Screenshots/1.png " ")

5. Клонировать свой личный удалённый репозиторий на компьютер.
Клонирование удаленного репозитория делается, используя команду `git clone`.
Для дальнейшей работы с файлами осуществляется переход в директорию LR6 командой `cd LR6`.
![-](https://github.com/shadapovatsyrena/LR6/blob/master/Screenshots/2.png " ")

6. Добавить файл через интерфейс GitHub. Подтянуть изменения в локальный репозиторий.
Подтягивание изменения из веб-интерфейса GitHub для клиента Git с помощью команды `git pull`.
![-](https://github.com/shadapovatsyrena/LR6/blob/master/Screenshots/3.png " ")

7. Получить историю операций для каждой из веток.
Просмотр истории операций ветки master, используя команду `git log`.
![-](https://github.com/shadapovatsyrena/LR6/blob/master/Screenshots/4.png " ")
Переход в ветку branch1 командой `git checkout branch1`.
Просмотр коммитов ветки branch1 с помощью команды `git log`.
![-](https://github.com/shadapovatsyrena/LR6/blob/master/Screenshots/5.png " ")

8. Просмотреть последние изменения можно с помощью команды `git log -p`
![-](https://github.com/shadapovatsyrena/LR6/blob/master/Screenshots/6.png " ")

9. Выполнить слияние в ветку master, разрешив конфликт.
Перед выполнением слияния необходимо вернуться в метку master с помощью команды `git checkout master`. Для слияния используется команда `git merge branch1`
![-](https://github.com/shadapovatsyrena/LR6/blob/master/Screenshots/7.png " ")
Так как файл mergefile.txt не отслеживается, используется команда `git status` для отображения состояния рабочего каталога.
Добавление файла mergefile.txt с помощью команды `git add`.
![-](https://github.com/shadapovatsyrena/LR6/blob/master/Screenshots/8.png " ")
![-](https://github.com/shadapovatsyrena/LR6/blob/master/Screenshots/9.png " ")

10. Удалить побочную ветку после успешного слияния.
Удаление побочной ветки осуществляется при помощи команды `git branch -d`.
![-](https://github.com/shadapovatsyrena/LR6/blob/master/Screenshots/10.png " ")

11. Сделать изменения и зафиксировать их, оставляя комментарии, несколько раз.
Название файла - file.txt.
После создания файла применяется команда `git status`. Видно, что файл file не отслеживается. 
Нужно добавить его с помощью команды `git add`.
Затем с помощью команды `git commit -m `добавляется коммит.
![-](https://github.com/shadapovatsyrena/LR6/blob/master/Screenshots/11.png " ")
Просмотр комментариев, используя команду `git log`.
![-](https://github.com/shadapovatsyrena/LR6/blob/master/Screenshots/12.png " ")

12. Сделать откат коммита.
Откат коммита осуществляется за счет команды `git reset --hard HEAD~1`.
![-](https://github.com/shadapovatsyrena/LR6/blob/master/Screenshots/13.png " ")

13. Создать ветку для отчёта.
Создание ветки для отчета и переход в эту ветку делается с помощью команд `git branch report` и `git checkout report`.
![-](https://github.com/shadapovatsyrena/LR6/blob/master/Screenshots/14.png " ")

14. Начать оформлять отчёт в файле README.md

15. Получить историю операций в форматированном виде (сокращённый хэш + дата + имя автора + комментарий). Добавить её в отчёт и сделать финальную фиксацию изменений.
![-](https://github.com/shadapovatsyrena/LR6/blob/master/Screenshots/15.png " ")

16. Отправить локальные изменения в сетевое хранилище GitHub.
Отправка изменений осуществляется командой git push.
