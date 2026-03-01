# Шаблон для html верстки на gulp и pug

Под указанную ниже структуру настроена сборка https://github.com/web-bombaster/My-Gulp-Project-Builder. Но вы можете переопределить конфиг под ваши нужды.


```text
├─ dist/    ← сюда всё собирается при билде
├─ src/
│   ├─ assets/
│   │   ├─ fonts/    ← закидываем сразу woff2 шрифты
│   │   │   └─ ...
│   │   ├─ icons/
│   │   │   └─ ...
│   │   ├─ images/
│   │   │   └─ ...
│   │   └─ libs/    ← для подключаемых библиотек
│   │       └─ ...
│   ├─ js/
│   │   ├─ myscripts
│   │   │   ├─ helpers.js
│   │   │   └─ ...
│   │   └─ common.js    ← сюда инклюдим скрипты из myscripts
│   ├─ libs/
│   │   └─ libs-includ.js    ← сюда инклюдим скрипты библиотек из src/assets/libs/
│   ├─ pug/
│   │   ├─ bloks/    ← сюда добавляем блоки
│   │   │   ├─ head.pug
│   │   │   ├─ header.pug
│   │   │   ├─ footer.pug
│   │   │   └─ ...
│   │   ├─ components/    ← сюда добавляем компоненты
│   │   │   ├─ button.pug
│   │   │   └─ ...
│   │   └─ pages/    ← сюда добавляем страницы
│   │       ├─ index.pug
│   │       ├─ about.pug
│   │       └─ ...
│   └─ scss/
│       ├─ base/    ← базовые стили (не блоки и не компоненты)
│       │   ├─ _fonts.scss
│       │   ├─ _main.scss
│       │   ├─ _normalize.scss
│       │   ├─ _vars.scss
│       │   ├─ _verstka.scss    ← стили для страницы-меню для показа верстки
│       │   └─ ...
│       ├─ blocks/    ← блоки
│       │   ├─ _footer.scss
│       │   └─ ...
│       ├─ components/    ← компоненты
│       │   ├─ _burger.scss
│       │   ├─ _button.scss
│       │   └─ ...
│       └─ main.scss    ← тут делаем импорты всех других scss
├─ .gitignore
└─ README.md
```