# Отчет
### Сайт:
https://daniyarirkagaliev.github.io/site4/

### package.json
https://github.com/DaniyarIrkagaliev/site4/blob/main/package.json
#### Добавленные и измененные скрипты:
1. "normalize-styles" (17 строка) - я использоал normalize.css - CSS-файл, который обеспечивает для HTML-элементов лучшую кроссбраузерность в стилях по умолчанию, "A modern alternative to CSS resets", как они сами пишут у себя в репозитории
Из-за этого появилась необходимость продублировать скрипт "styles" под этот файл. Значительных изменений в скриптах нет
2. "copy-images" (18 строка) - у меня используются изображения, их тоже необходимо перенести на сайт
3. "build" (19 строка) - добавлено выполнение указанных выше скриптов

### deploy.yml 
https://github.com/DaniyarIrkagaliev/site4/blob/main/.github/workflows/deploy.yml
#### Шаги
1. Билд (19 строка),
2. Создается папка под содержимое сайта (22 строка),
3. Копируется сбилженное в папку сайта (24 строка),
4. Деплой (28 строка)<br>
4.1. Папка переносится на gh-pages ветку (34-35 строки)

### Итог
Два html документа [index.html](https://github.com/DaniyarIrkagaliev/site4/blob/gh-pages/index.html) и [secondPage.html](https://github.com/DaniyarIrkagaliev/site4/blob/gh-pages/secondPage.html), стили в папке [css](https://github.com/DaniyarIrkagaliev/site4/tree/gh-pages/css) и [набор изображений](https://github.com/DaniyarIrkagaliev/site4/tree/gh-pages/images) после Build переносятся на [gh-pages btanch](https://github.com/DaniyarIrkagaliev/site4/tree/gh-pages), [сайт на Github Pages](
https://daniyarirkagaliev.github.io/site4/) создается на основе данного branch.
html файлы [минифицируются](https://github.com/DaniyarIrkagaliev/site4/blob/main/package.json "15 строка") (подсказка при наведении)
В html файлах имеются footer, header, meta-теги
