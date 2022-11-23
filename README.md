# my-gulp-build
 Моя сборка таск-менеджера для проектов.

 Выполяет следующие функции:
 - переделывает SCSS в CSS
 - мимифицирует HTML, JS, CSS код
 - копирует медиа-файлы из папки media
 - запускает автообновляющийся локальный сервер

Структура проектов:

    Project folder/
     ├─── dist/
     |     ├─── media/
     |     |     ├─── images/
     |     |     └─── fonts/
     |     ├─── js/
     |     |     ├─── code.js
     |     |     └─── code.min.js
     |     ├─── index.html
     |     └─── main.min.css
     └─── src/
           ├─── media/
           |     ├─── images/
           |     └─── fonts/
           ├─── js/
           |     └─── code.js
           ├─── scss/
           |     ├─── blocks/
           |     ├─── modifications/
           |     └─── main.scss
           └─── index.html

Примечания:
- index.html обращается к main.min.css
- все обращения идут через "../" и дальше от уровня, в котором располагается index.html (от корня версии проекта)
- для установки переместить файлы gulpfile.js и pacage.json в проект и прописать в терминале npm i
- для запуска прописать в терминал "gulp"
