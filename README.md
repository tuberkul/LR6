# LR6
Лабораторная работа №6

**Цель лабораторной работы:** изучение базовых возможностей системы
управления версиями, опыт работы с Git Api, опыт работы с локальным и
удаленным репозиторием. 

**Ход работы:**
Вошел в свой ранее созданный [аккаунт](https://github.com/tuberkul/) на GitHub и сделал копию в личное хранилище из https://github.com/Kurtyanik/LR6/.<br>
Следом я установил Git и настроил клиент командами git config --global user.name "4917 Moshkin N. A." и git config --global user.email 120nik01@mail.ru<br>
Далее я клонировал удаленный репозиторий на компьютер командой git clone https://github.com/Kurtyanik/LR6/<br>
Все предыдущие пункты продемонстрированы на рисунке 1.<br>
	![Рисунок 1](/screenshots/1.png)<br>
	Рисунок 1. Настройка клиента и клонирование репозитория<br>
Следующим шагом я перешел в ветку branch1, добавил файл и отредактировал его (через интерфейс GitHub). Далее подтянул изменения в локальный репозиторий.<br>
При этом я использовал команды cd LR6, чтобы зайти в локальный репозиторий, git checkout branch1, чтобы перейти в побочную ветку и подтянул изменения с помощью команды pit pull https://github.com/tuberkul/LR6/ branch1<br>
Все это я продемонстрировал ниже на рисунках 2-5.<br>
	![Рисунок 2](/screenshots/2.png)<br>
	Рисунок 2. Добавление и редактирование файла<br>
	![Рисунок 3](/screenshots/3.png)<br>
	Рисунок 3. Подтверждение добавления файла<br>
	![Рисунок 4](/screenshots/4.png)<br>
	Рисунок 4. Файл в ветке branch1<br>
	![Рисунок 5](/screenshots/5.png)<br>
	Рисунок 5. Переход во вторую ветку и подтягивание изменений<br>
Далее я получил историю операций для каждой из веток с помощью команды git log<br>
	![Рисунок 6](/screenshots/6.png)<br>
	Рисунок 6. История операций в ветке branch1<br>
	![Рисунок 7](/screenshots/7.png)<br>
	Рисунок 7. История операций в ветке master<br>
Следом я выполняю слияние в ветку master, вручную разрешив конфликт. Для этого я использовал команды git merge branch1 (в ветке master), vim mergefile.txt (чтобы открыть конфликтующий файл), git add mergefile.txt и git commit.<br>
Этапы видны на следующих рисунках (8-10):<br>
	![Рисунок 8](/screenshots/8.png)<br>
	Рисунок 8. Ввод команды слияния и открытие в редакторе конфликтующего файла<br>
	![Рисунок 9](/screenshots/9.png)<br>
	Рисунок 9. Отредактированный файл<br>
	![Рисунок 10](/screenshots/10.png)<br>
	Рисунок 10. Подтверждение изменения файла<br>
После успешного слияния я удаляю ветку branch1 командами git branch -D branch1 для удаления в локальном репозитории и git push https://github.com/tuberkul/LR6/ --delete branch1 для удаления в удаленном репозитории.<br>
Можно увидеть выполнение этого пункта на рисунке 11:
	![Рисунок 11](/screenshots/11.png)<br>
	Рисунок 11. Удаление ветки branch1<br>
Заодно я удалил ненужные ветки отчетов других студентов последней упомянутой командой (только с изменением названий веток).
Видно это ниже на рисунке 12.
	![Рисунок 12](/screenshots/12.png)<br>
	Рисунок 12. Удаление ненужных веток<br>
Применил все изменения в ветке master к удаленному репозиторию с помощью команды git push https://github.com/tuberkul/LR6/ master<br>
Выполнение этого пункта видно на рисунке 13:
	![Рисунок 13](/screenshots/13.png)<br>
	Рисунок 13. Применение изменений в ветке master к удаленному репозиторию<br>
Далее я создаю два файла (file1.txt и file2.txt), по очереди делая коммиты их создания. Для этого я использовал команды vim \*название файла\*, git add \*название файла\* и git commit -m '\*комментарий\*'<br>
Продемонстрировал эти шаги на рисунках 14-17:<br>
	![Рисунок 14](/screenshots/14.png)<br>
	Рисунок 14. Редактирование файла 1<br>
	![Рисунок 15](/screenshots/15.png)<br>
	Рисунок 15. Коммит вышеупомянутого действия<br>
	![Рисунок 16](/screenshots/16.png)<br>
	Рисунок 16. Редактирование файла 2<br>
	![Рисунок 17](/screenshots/17.png)<br>
	Рисунок 17. Коммит вышеупомянутого действия<br>
Делаю хард откат одного коммита командой git reset --hard HEAD~1<br>
Это продемонстрировано ниже на рисунке 18.<br>
	![Рисунок 18](/screenshots/18.png)<br>
	Рисунок 18. Откат последнего коммита<br>
Следом получил лог в форматированном виде командой git log --pretty=format:"%h : %ad; %an %s"<br>
Это можно увидеть на рисунке 19:<br>
	![Рисунок 19](/screenshots/19.png)<br>
	Рисунок 19. Лог в форматированном виде<br>
Далее получил полный лог, зайдя в папку .git/logs и открыв файл HEAD в блокноте. Это видно на рисунке 20:
	![Рисунок 20](/screenshots/20.png)<br>
	Рисунок 20. Полный лог<br>
Следующим шагом я создал ветку для отчета командой git ckeckout -b report<br>
Продемонстрировал данный шаг на рисунке 21:<br>
	![Рисунок 21](/screenshots/21.png)<br>
	Рисунок 21. Создание ветки для отчета<br>
Далее я оформил отчет в файле README.md в блокноте, используя markdown синтаксис.<br>
Следом я добавил практически все скриншоты и коммитнул их. Для этого использовал команды git add screenshots/\* и git commit -m 'Добавил практически все скриншоты'<br>
Это видно на рисунке 22:
	![Рисунок 22](/screenshots/22.png)<br>
	Рисунок 22. Добавление и коммит практически всех скриншотов<br>
Последним шагом я отправляю локальные изменения в сетевое хранилище GitHub (в каждой ветке). Для этого я использовал команды git add \*, git commit -m 'Сделал отчет и загрузил оставшиеся скриншоты' git push https://github.com/tuberkul/LR6/ \*название ветки\*<br>
Это видно на рисунках 23 и 24:
	![Рисунок 23](/screenshots/23.png)<br>
	Рисунок 23. Отправка локальных изменений на сервера GitHub<br>
	![Рисунок 24](/screenshots/24.png)<br>
	Рисунок 24. Отправка локальных изменений на сервера GitHub<br>

**Вывод:** изучил базовые возможности системы управления версиями, получил опыт работы с Git Api, а также опыт работы с локальным и удаленным репозиторием.