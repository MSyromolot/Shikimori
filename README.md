# Shikimori — кастомное оформление профиля

CSS-тема для [Shikimori](https://shikimori.io). Содержимое `main.css` вставляется в настройки оформления профиля.

## Структура

```
main.css                  ← точка входа: переменные + @import
├── background.css        ← фон страницы (body)
├── colors.css            ← тёмная тема контентных блоков
├── global.css            ← глобальные скругления
├── top-menu.css          ← закреплённое верхнее меню
├── avatar.css            ← кастомный аватар (GIF через ::before)
├── profile-head.css      ← сетка шапки профиля
├── stats-lists.css       ← кнопки списков аниме / манги
├── lifetime.css          ← блок «время за аниме и мангой»
├── achievements.css      ← скругления достижений и бейджей
├── achievement-posters.css ← замена картинок конкретных ачивок
├── other.css             ← боковая колонка достижений
├── activityBar.css       ← анимация графика активности (внешний)
└── sortAnimeInCollection.css ← сортировка аниме в коллекциях (опционально)
```

## Настройка

Все параметры — в блоке `:root` файла `main.css`:

| Переменная | Описание |
|---|---|
| `--background-url` | Фоновое изображение страницы |
| `--avatar-url` | GIF/картинка аватара |
| `--avatar-border-radius` | Скругление аватара |
| `--page-background` | Фон контентных блоков |
| `--anime-stat-bg` / `--manga-stat-bg` | Цвета кнопок списков |
| `--radius-sm/md/lg` | Скругления элементов |
| `--achivment-*` | Настройки модуля прогрессбара ачивок (kaurkaur) |

## Опциональные модули

Раскомментируйте `@import` в `main.css`:

- `sortAnimeInCollection.css` — сортировка аниме по статусу в коллекциях
