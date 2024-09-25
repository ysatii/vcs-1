# Домашнее задание к занятию «Системы контроля версий» - Мельник Юрий Александрович
## Задание 1. Создать и настроить репозиторий для дальнейшей работы на курсе
<details>
<summary>Нажмите для просмотра задания</summary>
В рамках курса вы будете писать скрипты и создавать конфигурации для различных систем, которые необходимо сохранять для будущего использования. 
Сначала надо создать и настроить локальный репозиторий, после чего добавить удалённый репозиторий на GitHub.

### Создание репозитория и первого коммита

1. Зарегистрируйте аккаунт на [https://github.com/](https://github.com/). Если предпочитаете другое хранилище для репозитория, можно использовать его.
2. Создайте публичный репозиторий, который будете использовать дальше на протяжении всего курса, желательное с названием `devops-netology`.
   Обязательно поставьте галочку `Initialize this repository with a README`. 
   
    ![Диалог создания репозитория](img/github-new-repo-1.jpg)
    
3. Создайте [авторизационный токен](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) для клонирования репозитория.
4. Склонируйте репозиторий, используя протокол HTTPS (`git clone ...`).
 
    ![Клонирование репозитория](img/github-clone-repo-https.jpg)
    
5. Перейдите в каталог с клоном репозитория (`cd devops-netology`).
6. Произведите первоначальную настройку Git, указав своё настоящее имя, чтобы нам было проще общаться, и email (`git config --global user.name` и `git config --global user.email johndoe@example.com`). 
7. Выполните команду `git status` и запомните результат.
8. Отредактируйте файл `README.md` любым удобным способом, тем самым переведя файл в состояние `Modified`.
9. Ещё раз выполните `git status` и продолжайте проверять вывод этой команды после каждого следующего шага. 
10. Теперь посмотрите изменения в файле `README.md`, выполнив команды `git diff` и `git diff --staged`.
11. Переведите файл в состояние `staged` (или, как говорят, просто добавьте файл в коммит) командой `git add README.md`.
12. И ещё раз выполните команды `git diff` и `git diff --staged`. Поиграйте с изменениями и этими командами, чтобы чётко понять, что и когда они отображают. 
13. Теперь можно сделать коммит `git commit -m 'First commit'`.
14. И ещё раз посмотреть выводы команд `git status`, `git diff` и `git diff --staged`.

### Создание файлов `.gitignore` и второго коммита

1. Создайте файл `.gitignore` (обратите внимание на точку в начале файла), проверьте его статус сразу после создания. 
1. Добавьте файл `.gitignore` в следующий коммит (`git add...`).
1. На одном из следующих блоков вы будете изучать `Terraform`, давайте сразу создадим соотвествующий каталог `terraform` и внутри этого каталога — файл `.gitignore` по примеру: https://github.com/github/gitignore/blob/master/Terraform.gitignore.  
1. В файле `README.md` опишите своими словами, какие файлы будут проигнорированы в будущем благодаря добавленному `.gitignore`.
1. Закоммитьте все новые и изменённые файлы. Комментарий к коммиту должен быть `Added gitignore`.

### Эксперимент с удалением и перемещением файлов (третий и четвёртый коммит)

1. Создайте файлы `will_be_deleted.txt` (с текстом `will_be_deleted`) и `will_be_moved.txt` (с текстом `will_be_moved`) и закоммите их с комментарием `Prepare to delete and move`.
1. В случае необходимости обратитесь к [официальной документации](https://git-scm.com/book/ru/v2/Основы-Git-Запись-изменений-в-репозиторий) — здесь подробно описано, как выполнить следующие шаги. 
1. Удалите файл `will_be_deleted.txt` с диска и из репозитория. 
1. Переименуйте (переместите) файл `will_be_moved.txt` на диске и в репозитории, чтобы он стал называться `has_been_moved.txt`.
1. Закоммитьте результат работы с комментарием `Moved and deleted`.

### Проверка изменения

1. В результате предыдущих шагов в репозитории должно быть как минимум пять коммитов (если вы сделали ещё промежуточные — нет проблем):
    * `Initial Commit` — созданный GitHub при инициализации репозитория. 
    * `First commit` — созданный после изменения файла `README.md`.
    * `Added gitignore` — после добавления `.gitignore`.
    * `Prepare to delete and move` — после добавления двух временных файлов.
    * `Moved and deleted` — после удаления и перемещения временных файлов. 
2. Проверьте это, используя комманду `git log`. Подробно о формате вывода этой команды мы поговорим на следующем занятии, но посмотреть, что она отображает, можно уже сейчас.

### Отправка изменений в репозиторий

Выполните команду `git push`, если Git запросит логин и пароль — введите ваши логин и пароль от GitHub. 

В качестве результата отправьте ссылку на репозиторий. 
</details>

## Решение 1. Создать и настроить репозиторий для дальнейшей работы на курсе

 
### Создание репозитория и первого коммита
1. Аккаунт  на https://github.com/ уже зарегистрирован  
![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1.jpg)

2. Создадим  публичный репозиторий, с названием **devops-netology**. Обязательно ставим галочку **Initialize this repository with a README**.
![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_1.jpg)
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_2.jpg)

3. Создадим авторизационный токен для клонирования репозитория.
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_3.jpg)
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_4.jpg)
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_5.jpg)
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_6.jpg)
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_7.jpg)
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_8.jpg)
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_9.jpg)


4. Склонируем репозиторий, используя протокол HTTPS (git clone ...).
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_10.jpg)
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_11.jpg)

5. Перейдем  в каталог с клоном репозитория (**cd devops-netology**).
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_12.jpg)


 Произведём первоначальную настройку Git, указав своё настоящее имя, чтобы нам было проще общаться, и email (git config --global user.name и git config --global user.email johndoe@example.com).
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_13.jpg)

 Выполним команду git status и запомним результат.

6. Отредактируем файл README.md, тем самым переведя файл в состояние Modified.
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_14.jpg)


 Ещё раз выполним **git status** и продолжаем проверять вывод этой команды после каждого следующего шага.

  Теперь посмотрим изменения в файле README.md, выполнив команды git diff и git diff --staged.

  Переведим файл в состояние staged (или, как говорят, просто добавьте файл в коммит) командой git add README.md.

7. И ещё раз выполним команды git diff и git diff --staged.  
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_15.jpg)

8. Теперь можно сделать коммит git commit -m 'First commit'.

9. И ещё раз посмотреть выводы команд git status, git diff и git diff --staged.  
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_16.jpg)



## Создание файлов .gitignore и второго коммита

1. Создадим файл .gitignore  
2. Добавим файл .gitignore в следующий коммит (git add...).  
3. Cоздадим соотвествующий каталог terraform и внутри этого каталога — файл .gitignore по примеру: https://github.com/github/gitignore/blob/master/Terraform.gitignore.  
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image2.jpg)
4. В файле README.md опишите своими словами, какие файлы будут проигнорированы в будущем благодаря добавленному .gitignore.  
5. Закоммитим все новые и изменённые файлы. Комментарий к коммиту должен быть Added gitignore.  


 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image2_1.jpg)

 **terraform/.gitignore** - позволить временным и служебным файлам не попасть в git репозиторий, игнорируруемые файлы большого размера и каждый раз при выполнение кода террафом будут созданы заново. Хранить их в каком либо репозитории не имеет смысла! Также это могут быть файлы-ключи содержащие какую ту информацию включая токены которые не должны попасть в открытое пространство!

 
## Эксперимент с удалением и перемещением файлов (третий и четвёртый коммит)

1. Создайте файлы will_be_deleted.txt (с текстом will_be_deleted) и will_be_moved.txt (с текстом will_be_moved) и закоммите их с комментарием Prepare to delete and move.
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image3.jpg)
2. В случае необходимости обратитесь к официальной документации — здесь подробно описано, как выполнить следующие шаги.
3. Удалите файл will_be_deleted.txt с диска и из репозитория.
4. Переименуйте (переместите) файл will_be_moved.txt на диске и в репозитории, чтобы он стал называться has_been_moved.txt.
5. Закоммитьте результат работы с комментарием Moved and deleted.


## Проверка изменения

1. В результате предыдущих шагов в репозитории должно быть как минимум пять коммитов  
      -  Initial Commit — созданный GitHub при инициализации репозитория.
      -  First commit — созданный после изменения файла README.md.
      -  Added gitignore — после добавления .gitignore.
      -  Prepare to delete and move — после добавления двух временных файлов.
      -  Moved and deleted — после удаления и перемещения временных файлов.
2. Проверим это, используя комманду git log.  

 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image3_1.jpg)


## Отправка изменений в репозиторий

Выполним команду **git push** .

В качестве результата отправьте ссылку на репозиторий.  
репозиторий https://github.com/ysatii/devops-netology Создан!

 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image4.jpg)

 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image4_1.jpg)

