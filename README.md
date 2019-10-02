##link https://natalizag.github.io/Test_28_10_19/
#Базовая структура проекта с настроенными webpack, less, babel
Для использования скачать, разархивировать, и выполнить следующие команды в терминал(командной строке)
1. npm install
2. npm start -команда которая запустит dev сервер, необходимо для авоматической компиляции scss/ES6 файлов
3. Перейти в браузере по адресу http://localhost:8080
4. Для остановки дев сервера в консоле(терминале) необходимо нажать два раза CTRL+C
Если возникают ошибки компиляции то в терминале будут красные
сообщения об ошибке, в самом начале сообщения достаточно
точно описывается что пошло не так, обращайте на это внимание. Так же в случае проблем со сборкой просьба к вопросу прикладывать скриншот с текстом ошибки консоли

### Файловая структура

assets - дирректория для хранения асеетов - шрифты изображения пример использования смотреть в common/styles/header.less
###
``` 
src
.
|
├──index - старница index.html и все что к ней относится
|   |
|   +-- scripts - скрипты, обязательно необходимо импортить в index.js  
|   +-- styles - все стили разделенные по файлам, так же необходимо импортить в index.scss
|   +-- index.html - основной документ html, домашняя страница вашего сайта
|   +-- index.js - главный фаил js, весь скрипт который относится к данной странице импортится в данном файле(из дирректории scripts)
|   +-- index.scss - основной фаил стилей
+- common - дирректория в которой хранятся общие файлы для всех страниц вашего сайта например стили и скрипты для использования нужно имопртить в главных файла страниц смотреть index/index.scss
    |
    +- scripts
    |
    +- styles     
```
### Добавление новой страницы
Выполнить команду `npm run page:add [имя страницы]`
например `npm run page:add lesson_5` - создаст новую старницу lesson_5
### Удаление страницы
`npm run page:remove [имя страницы]`

#### SCSS
`npm run page:add [имя страницы] -- --styles=scss` - добавит новую старницу с scss

<br/> Для перехода на другие страницы не index, в адресной строке добавить к http://localhost:8080 /имя_страницы.html например http://localhost:8080/about.hml
