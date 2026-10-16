# Мої 3 найкращі міста світу

Лабораторна робота №1 з дисципліни «WEB-програмування».
Автор: Кушнір Андрій Назарович, група КН-41.

Статичний багатосторінковий блог на чистому HTML: без CSS і JavaScript.

**Сайт:** https://teitp.github.io/my-best-cities/  
**Репозиторій:** https://github.com/TeITp/my-best-cities

## Структура проєкту
```
my-best-cities/
├── index.html          головна: вступ, рейтинг, таблиця порівняння
├── city-lviv.html      Львів
├── city-madrid.html    Мадрид
├── city-london.html    Лондон
├── form.html           форма «Запропонувати місто»
├── images/
│   ├── lviv.jpg
│   ├── madrid.jpg
│   └── london.jpg
└── README.md
```

## Sitemap
```
                 index.html
        ┌────────┬───┴────┬──────────┐
        ↓        ↓        ↓          ↓
 city-lviv  city-madrid  city-london  form.html
        └────────┴────────┴──────────┘
          усі сторінки мають однакове меню
          і посилання «На головну»
```

## Використані HTML-елементи
- Структура: `header`, `nav`, `main`, `section`, `article`, `figure`/`figcaption`, `footer`.
- Контент: `h1`–`h3` (по одному `h1` на сторінку), `p`, `ul`, `ol`, `table` з `caption`/`thead`/`th scope`, `meter`, `time`, `abbr`.
- Посилання: тільки відносні (`city-lviv.html`), зовнішні ведуть на Вікіпедію з `target="_blank" rel="noopener noreferrer"`. Поточна сторінка в меню позначена `aria-current="page"`.
- Форма: `fieldset`/`legend`, `label[for]`↔`input[id]`, поля `text`, `email`, `number`, `radio`, `checkbox`, `datalist`, `select`/`option`, `textarea`, кнопки `submit` і `reset`. 7 полів мають `required`, у кожного поля є `name`.

## Git і GitHub
```bash
cd my-best-cities
git init
git add .
git commit -m "Initial project structure"
git branch -M main
git remote add origin https://github.com/TeITp/my-best-cities.git
git push -u origin main
```
Краще робити кілька змістовних комітів, а не один, наприклад: `Add home page`, `Add city pages`, `Add suggestion form`, `Add README`.

## GitHub Pages
Settings → Pages → Build and deployment → Source: **Deploy from a branch** → Branch: `main`, папка `/ (root)` → **Save**.
Сайт з'явиться за кілька хвилин за адресою https://teitp.github.io/my-best-cities/.

## Джерела фотографій
- `images/lviv.jpg` — Jorge Láscar, [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Northern_side_of_the_Market_Square_Cropped.jpg), CC BY-SA 3.0
- `images/madrid.jpg` — Jorge Franganillo, [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Madrid_Plaza_Mayor_(48733706273).jpg), CC BY 2.0
- `images/london.jpg` — ThatsTheBoss, [Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Palace_of_Westminster_as_seen_from_Westminster_Bridge.jpg), CC0

Фото зменшено до 480 px завширшки.
