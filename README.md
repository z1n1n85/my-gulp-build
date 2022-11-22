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
 |     |     ├─── _images_/
 |     |     └─── _fonts_/
 |     ├─── js/
 |     |     ├─── _code.js_
 |     |     └─── code.min.js
 |     ├─── index.html
 |     └─── main.min.css
 └─── src/
       ├─── media/
       |     ├─── _images_/
       |     └─── _fonts_/
       ├─── js/
       |     └─── code.js
       ├─── scss/
       |     ├─── _blocks_/
       |     ├─── _modifications_/
       |     └─── main.scss
       └─── index.html

Примечания:
- index.html обращается к main.min.css
- все обращения идут через "../"