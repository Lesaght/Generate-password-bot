# Password Generator Bot 🤖

Бот для генерации безопасных случайных паролей прямо в Telegram. Поддерживает настройку длины, использование цифр и символов, а также переключение между русским и английским языками.

![Telegram Bot Example](https://via.placeholder.com/468x300?text=Password+Generator+Bot+Preview)

## Особенности ✨

- **Генерация паролей с настраиваемой длиной** (по умолчанию 12 символов)
- **Опция включения/выключения цифр и специальных символов**
- **Поддержка двух языков:** русский 🇷🇺 и английский 🇬🇧
- **Интуитивный интерфейс** с inline-кнопками
- **Защита от некорректного ввода** (например, нечисловых значений для длины)

## Установка и запуск 🚀

1. **Клонируйте репозиторий:**

   ```bash
   git clone https://github.com/Lesaght/Generate-password-bot
   cd password_bot
   ```

2. **Установите зависимости:**

   ```bash
   pip install pyTelegramBotAPI
   ```

3. **Создайте бота через [@BotFather](https://t.me/BotFather) и получите токен.**

4. **Замените `TELEGRAM_BOT_TOKEN` в файле `password_bot.py` на ваш токен:**

   ```python
   BOT_TOKEN = 'ВАШ_ТОКЕН_ЗДЕСЬ'
   ```

5. **Запустите бота:**

   ```bash
   python password_bot.py
   ```

## Использование 📝

### Основные команды

- `/start` — начать работу с ботом.
- `/help` — показать список команд.
- `/options` — открыть настройки генерации пароля.

### Настройки пароля

После запуска бота нажмите `/options` для смены настроек:

- **Длина:** Изменить длину пароля (число > 0).
- **Цифры/Символы:** Включить или выключить использование цифр и специальных символов.
- **Сгенерировать пароль:** Получить пароль с текущими настройками.
- **Язык:** Переключить между русским и английским интерфейсом.

### Примеры взаимодействия

**Установка длины пароля:**

- Пользователь нажимает кнопку **"Длина: 12"**
- Бот отправляет: **"Введите новую длину пароля..."**
- Пользователь вводит **"16"**
- Бот отвечает: **"Длина пароля установлена на 16."**

**Генерация пароля:**

- Бот отправляет сообщение: **"Генерирую пароль..."**
- Результат: **"Сгенерированный пароль: `x7@k!qLZ$vT4^fY9`"**

## Локализация 🌍

Для смены языка нажмите кнопку **Язык | Language** в меню настроек и выберите:
- **English** — английский интерфейс
- **Русский** — русский интерфейс

## Технические детали ⚙️

Генерируемый пароль включает:
- Буквы (верхний и нижний регистр)
- Цифры (если включено)
- Специальные символы (например, !@#$%^&*() и другие, если включено)

Пароль отправляется в формате **MarkdownV2** для корректного отображения в Telegram.

## Лицензия 📄

Проект распространяется под лицензией **MIT**. Подробности см. в файле [LICENSE](LICENSE).
