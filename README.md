# NuffViewer

Forgot your password? Use **NuffViewer**! This script will help you recover all your passwords and accounts!

## Описание

NuffViewer — это инструмент для извлечения сохранённых данных из популярных браузеров и системных учетных данных Windows. Он извлекает пароли, cookies, историю посещений и данные автозаполнения, сохраняя всё в удобный текстовый файл с временной меткой.

Поддерживаемые браузеры:
- Google Chrome
- Microsoft Edge
- Opera GX
- Opera
- Yandex Browser
- Brave
- Vivaldi
- Mozilla Firefox

Также извлекает учетные данные Windows (Windows Credentials).

## Установка

1. Убедитесь, что у вас установлен Python 3.7 или выше.
2. Склонируйте репозиторий:
   ```bash
   git clone https://github.com/ваш_юзернейм/NuffViewer.git
   cd NuffViewer

Установите зависимости:
bash

pip install -r requirements.txt

Использование
Запустите скрипт:
bash

python nuffviewer.py

После выполнения данные будут сохранены в файл вида extracted_data_YYYYMMDD_HHMMSS.txt в той же директории.

Откройте файл, чтобы просмотреть извлечённые данные в табличном формате.

Пример вывода

=== Chrome Passwords ===
-----------------------------------------
| URL               | Username | Password |
-----------------------------------------
| https://example.com | user1    | pass123|
-----------------------------------------

=== Firefox History ===
-------------------------------------------------------
| URL               | Title    | Visits | Last Visit      |
-------------------------------------------------------
| https://site.com  | Site     | 5      | 2023-10-01 12:00|
-------------------------------------------------------

Требования
ОС: Windows (из-за использования win32crypt и win32cred).

Установленные браузеры (данные извлекаются из локальных профилей).

Python 3.7+.

Зависимости из requirements.txt.

Примечания
Скрипт создаёт временные копии баз данных браузеров и удаляет их после обработки.

Используйте с осторожностью: данные сохраняются в открытом виде.

Работает только на Windows из-за зависимости от WinAPI.

Лицензия
MIT License. Используйте на свой страх и риск.
Created by @NuffLik

