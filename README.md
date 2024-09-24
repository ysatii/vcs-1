# Домашнее задание к занятию «Системы контроля версий» - Мельник Юрий Александрович


## Задание 1

### `Создайте виртуальную машину в Yandex Compute Cloud и с помощью Yandex Monitoring создайте дашборд, на котором будет видно загрузку процессора`
## `Процесс выполнения`
 

## Задание 1. Создать и настроить репозиторий для дальнейшей работы на курсе

 
### Создание репозитория и первого коммита
1. Аккаунт  на https://github.com/ уже зарегистрирован  
![alt text](https://github.com/ysatii/vcааs-1/blob/main/img/image1.jpg)

2. Создадим  публичный репозиторий, с названием **devops-netology**. Обязательно ставим галочку **Initialize this repository with a README**.
![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_1.jpg)
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_2.jpg)

3. Создайте авторизационный токен для клонирования репозитория.
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_3.jpg)
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_4.jpg)
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_5.jpg)
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_6.jpg)
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_7.jpg)
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_8.jpg)
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_9.jpg)


4. Склонируйте репозиторий, используя протокол HTTPS (git clone ...).
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_10.jpg)
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_11.jpg)

5. Перейдите в каталог с клоном репозитория (**cd devops-netology**).
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_12.jpg)


 Произведите первоначальную настройку Git, указав своё настоящее имя, чтобы нам было проще общаться, и email (git config --global user.name и git config --global user.email johndoe@example.com).
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_13.jpg)

 Выполните команду git status и запомните результат.

6. Отредактируйте файл README.md любым удобным способом, тем самым переведя файл в состояние Modified.
 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image1_14.jpg)


 Ещё раз выполните git status и продолжайте проверять вывод этой команды после каждого следующего шага.

  Теперь посмотрите изменения в файле README.md, выполнив команды git diff и git diff --staged.

  Переведите файл в состояние staged (или, как говорят, просто добавьте файл в коммит) командой git add README.md.

7. И ещё раз выполните команды git diff и git diff --staged. Поиграйте с изменениями и этими командами, чтобы чётко понять, что и когда они отображают.  
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
5. Закоммитьте все новые и изменённые файлы. Комментарий к коммиту должен быть Added gitignore.  


 ![alt text](https://github.com/ysatii/vcs-1/blob/main/img/image2_1.jpg)

 terraform/.gitignore - позволить временным и служебным файлам не попасть в git репозиторий, игнорируруемые файлы большого размера и каждый раз при выполнение кода террафом будут созданы заново. Хранить их в каком либо репозитории не имеет смысла. Также это могут быть файлы-ключи содержащие какую ту информацию включая токены которые не должны попасть в открытое пространство!
 
