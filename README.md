# Simple Web Application

Это простое веб-приложение с одной большой кнопкой по центру экрана. При нажатии на кнопку появляется сообщение.

## Структура проекта

- **index.html** — основная HTML-страница
- **styles.css** — стили для оформления и центрирования кнопки
- **script.js** — логика для обработки нажатия на кнопку

## Как запустить

1. Скачайте или склонируйте этот репозиторий.
2. Откройте файл `index.html` в любом современном браузере.

## Как это работает

- На странице отображается большая кнопка по центру.
- При нажатии на кнопку появляется всплывающее сообщение (`alert`).

## Пример кода

### index.html
```html
<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Simple Web Application</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <div class="container">
        <button type="button" id="myButton">Нажмите на меня</button>
    </div>
    <script src="script.js"></script>
</body>
</html>
```

### styles.css
```css
body, html {
    height: 100%;
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: Arial, sans-serif;
    background: #f0f0f0;
}

.container {
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
}

#myButton {
    padding: 40px 80px;
    font-size: 2rem;
    border: none;
    border-radius: 12px;
    background: #4CAF50;
    color: white;
    cursor: pointer;
    transition: background 0.2s;
}

#myButton:hover {
    background: #388e3c;
}
```

### script.js
```javascript
document.getElementById('myButton').addEventListener('click', function() {
    alert('Вы нажали на эту кнопку!');
});
```