# 🍪 Установка темы MidnightCookie

## 📋 Что у вас есть

1. **`midnight-source.css`** - Исходный CSS файл с полными стилями
2. **`MidnightCookie.theme.css`** - Готовый файл темы для Discord
3. **`test-theme.html`** - Файл для тестирования CSS в браузере

## 🎯 Как работает CSS файл

### Структура `midnight-source.css`:

```css
:root {
  /* CSS переменные для настройки */
  --app-bg: linear-gradient(135deg, rgb(25, 20, 18), rgb(35, 25, 22));
  --midnight-primary: hsl(220, 15%, 12%);
  --midnight-accent: hsl(28, 80%, 60%);
  /* ... и много других */
}

/* Стили для элементов Discord */
.app-2rEoOp { /* Фон приложения */ }
.sidebar-1tnWFu { /* Боковая панель */ }
.channel__972a0 { /* Каналы */ }
.message__80c10 { /* Сообщения */ }
/* ... и другие */
```

### Основные компоненты:

- **🎨 Цветовая схема** - Полуночные синие тона + теплые коричневые акценты
- **🚀 Анимации** - fadeIn, slideIn, pulse эффекты
- **📱 Адаптивность** - Поддержка мобильных устройств
- **♿ Доступность** - Поддержка высокого контраста и уменьшенной анимации

## 🛠️ Установка в Discord

### Шаг 1: Установка BetterDiscord

1. Скачайте BetterDiscord с [официального сайта](https://betterdiscord.app/)
2. Установите для вашей версии Discord
3. Перезапустите Discord

### Шаг 2: Установка темы

1. Откройте Discord
2. Перейдите в **User Settings** (⚙️) → **BetterDiscord** → **Themes**
3. Нажмите **Open Themes Folder**
4. Скопируйте файл `MidnightCookie.theme.css` в папку тем
5. Перезапустите Discord
6. Активируйте тему в настройках

### Пути к папке тем:

- **Windows**: `%APPDATA%\BetterDiscord\themes\`
- **macOS**: `~/Library/Application Support/BetterDiscord/themes/`
- **Linux**: `~/.config/BetterDiscord/themes/`

## 🧪 Тестирование

### В браузере:
1. Откройте файл `test-theme.html` в браузере
2. Убедитесь, что CSS переменные работают
3. Проверьте анимации и hover эффекты

### В Discord:
1. Активируйте тему
2. Проверьте внешний вид каналов, сообщений, кнопок
3. Убедитесь, что анимации работают плавно

## ⚙️ Настройка цветов

### Основные переменные для изменения:

```css
:root {
  /* Основные цвета */
  --midnight-primary: hsl(220, 15%, 12%);      /* Основной цвет */
  --midnight-secondary: hsl(225, 12%, 15%);    /* Вторичный цвет */
  --midnight-accent: hsl(28, 80%, 60%);        /* Акцентный цвет */
  
  /* Фон приложения */
  --app-bg: linear-gradient(135deg, rgb(25, 20, 18), rgb(35, 25, 22));
  
  /* Скругления */
  --app-radius: 8px;                           /* Общий радиус */
  --button-radius: 18px;                       /* Радиус кнопок */
  --textarea-radius: 24px;                     /* Радиус полей ввода */
  
  /* Анимации */
  --transition-time: 300ms;                    /* Время переходов */
}
```

### Пример изменения цветов:

```css
:root {
  /* Синяя тема */
  --midnight-primary: hsl(220, 30%, 15%);
  --midnight-accent: hsl(200, 80%, 60%);
  
  /* Зеленая тема */
  --midnight-primary: hsl(120, 20%, 15%);
  --midnight-accent: hsl(120, 80%, 60%);
  
  /* Фиолетовая тема */
  --midnight-primary: hsl(280, 20%, 15%);
  --midnight-accent: hsl(280, 80%, 60%);
}
```

## 🔧 Устранение неполадок

### Тема не загружается:
1. ✅ Проверьте, что BetterDiscord установлен
2. ✅ Убедитесь, что файл в правильной папке
3. ✅ Перезапустите Discord
4. ✅ Проверьте консоль на ошибки

### Проблемы с отображением:
1. 🔍 Отключите другие темы
2. 🔍 Проверьте конфликты CSS
3. 🔍 Убедитесь, что Discord обновлен

### Медленная работа:
1. ⚡ Уменьшите `--app-blur` до 6px
2. ⚡ Отключите анимации в системе
3. ⚡ Упростите сложные эффекты

## 📱 Совместимость

- **Discord**: Все версии
- **BetterDiscord**: 1.0.0+
- **Операционные системы**: Windows, macOS, Linux
- **Браузеры**: Chrome, Firefox, Edge (для веб-версии)

## 🎨 Кастомизация

### Создание собственной темы:

1. Скопируйте `midnight-source.css`
2. Измените переменные в `:root`
3. Добавьте свои стили
4. Переименуйте файл

### Пример кастомизации:

```css
/* Добавление новых цветов */
:root {
  --my-custom-color: hsl(45, 100%, 50%);
  --my-gradient: linear-gradient(45deg, var(--midnight-primary), var(--my-custom-color));
}

/* Применение новых стилей */
.custom-element {
  background: var(--my-gradient);
  border: 2px solid var(--my-custom-color);
}
```

## 📚 Полезные ссылки

- [BetterDiscord Documentation](https://docs.betterdiscord.app/)
- [CSS Variables Guide](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties)
- [Discord CSS Classes](https://github.com/DiscordStyles/DiscordThemes)

## 🆘 Поддержка

Если у вас возникли проблемы:

1. 📖 Проверьте этот файл
2. 🔍 Посмотрите консоль Discord (F12)
3. 🐛 Создайте issue в репозитории
4. 💬 Обратитесь в Discord сервер поддержки

---

**Удачи с установкой! 🍪✨**
