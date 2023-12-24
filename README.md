- Превью: https://kseylo.github.io/qr-component/
## Установка:

Установка зависимостей
```
pnpm install
```

Запуск
```
pnpm dev
```

## Скриншоты:
![preview](screenshots/preview.png)
## Технологии которые использовал:
- HTML
- CSS

## Проблемы с которыми столкнулся:

- Впервые столкнулся с вариативными шрифтами(variable fonts), не знал как подключить/использовать

Решение:
```css
@font-face {
	/* Имя шрифта которое будет использоваться */
    font-family: 'Outfit'; 
    /* Путь к файлу, woff2 - сжатый формат файла шрифта */
    src: url('/public/fonts/Outfit-VariableFont_wght.woff2') format('woff2');
    /* Диапазон значений толщины */
    font-weight: 100 1000;
    /* Показывать альтернативный шрифт, а затем заменить на загруженный */
    font-display: swap;
}

:root {
	/* Использование шрифта в корневом элементе */
	font-family: 'Outfit', sans-serif;
}
```
