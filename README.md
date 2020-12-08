#Отчет о лабораторной работе №6
#Яснева Марина гр.4916

###Ход работы:
На GitHub'е сделала копию https://github.com/Kurtyanik/LR6/

С помощью команды cd Desktop/laba6 в консоли Git Bash переша в созданную на рабочем столе папку laba6

Использовала команду git init чтобы инициализировать гит в данной папке

![Git init](screens/Screenshot2.png)

Командой git remote add origin связала папку с удалённым репозиторием на сайте GitHub

![Git remote add origin](screens/Screenshot2.png)

Затем через графический интерфейс GitHub добавила новый файл file.txt в удалённый репозиторий и добавила его в ветку master

![Новый файл](screens/Screenshot3.png)

![Новый файл](screens/Screenshot4.png)

![Новый файл](screens/Screenshot5.png)

Пользуясь командой git pull origin master загрузила изменения из удалённого репозитория в локальный

![Git pull](screens/Screenshot6.png)

Командой git log получила список операций/коммитов

![git log](screens/Screenshot7.png)

Используя git show получила более подробную информацию по последнему изменению

![git show](screens/Screenshot8.png)

Командой _git checkout -t branch1_ переключилась на другую ветку branch

![git checkout](screens/Screenshot9.png)

Попыталась выполнить слияние веток master и branch1 командой git merge branch1 и получила ошибку

![Merge error](screens/Screenshot10.png)

Вручную изменила файл mergefile.txt, вызвавший ошибку слияния, и выполнила коммит

![Fix](screens/Screenshot11.png)

Выполнила слияние веток master и branch1 а затем удалила ветку branch1 

![Merge](screens/Screenshot12.png)

![Branch delete](screens/Screenshot13.png)

Запушила всё в удалённый репозиторий командой git push origin master 

![Push1](screens/Screenshot14.png)

Затем сделала несколько изменений, создала новые файлы

![New files](screens/Screenshot15.png)

![New files git](screens/Screenshot16.png)

Командой git reset --hard HEAD~1 выполнила откат последнего коммита 

![Hard reset](screens/Screenshot17.png)

Запушила изменённую ветку

![Push2](screens/Screenshot18.png)

![Push2 result](screens/Screenshot19.png)

Пользуясь командой git checkout -b report создала новую ветку report

![New branch](screens/Screenshot20.png)

Текущая история git log --graph. Аргумент --graph позволяет графически изобразить ветки и коммиты на них

![Git log2](screens/Screenshot21.png)

С помощью команды git add . подготовила все новые файлы в папке laba6 к пушу

![Git add .](screens/Screenshot23.png)

Запушила файлы скриншотов в удалённый репозиторий

![Git add .](screens/Screenshot25.png)

Оформление отчёта в файле README.md, используя блокнот

![Readme](screens/Screenshot27.png)


Лог команд из папки .git/logs

![Logs](screens/Screenshot26.png)

Финальный результат команды git log

![Git log3](screens/Screenshot28.png)

Все файлы скриншотов лежат в папке screens