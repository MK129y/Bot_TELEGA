# Bot_TELEGA
In fil's bot's
В папках представлены боты разного назначения

Бот с викторинами
Данный чат бот проводит викторины для участников.

Заявленный базовый функционал:

кнопочное меню
база данных
анализе ответов пользователей
Бот работает с версиями Python 3.6+
С версиями ниже бот не работает!!!
Настройка для использования на личном ПК
Скачайте проект с гитхаба

Перейдите в папку с ботом с помощью консоли и команды cd <путь до проекта>

Установить зависимости из файла requirements.txt
Библиотеки к установке: requests, python-telegram-bot, python-dotenv, redis, vk-api.

Возможные команды для установки:
pip3 install -r requirements.txt
python -m pip install -r requirements.txt
python3.6 -m pip install -r requirements.txt

Создайте файл .env

Запишите в файл .env переменные: VKONTAKTE_GROUP_TOKEN=ваш_токен_группы вконтакте
TELEGRAM_TOKEN=ваш_токен_телеграм_бота
TELEGRAM_CHAT_ID=ваш_телеграм_айди
REDIS_PASSWORD=пароль_от_бд_redis
REDIS_ENDPOINT=ссылка_до_бд_redis
REDIS_PORT=порт_до_бд_redis

Запустите бота
Возможные команды для запуска(из консоли, из папки с ботом):

python3 vk_bot.py
python3 telegram_bot.py
или

python vk_bot.py
python telegram_bot.py
или

python3.6 main.py
python3.6 telegram_bot.py
Настройка для деплоя в облако Heroku
Если не знаем что такое Heroku - гуглим мануал или используем настройку бота из предыдущего туториала

Создайте app на Heroku
Перейдите в созданный app и выберите GitHub в качестве Deployment method
Укажите адрес до вашего!!! проекта на гитхабе
Зайдите в раздел Settings
Запишите в раздел Config Vars переменные KEY и VALUE: VKONTAKTE_GROUP_TOKEN=ваш_токен_группы вконтакте
TELEGRAM_TOKEN=ваш_токен_телеграм_бота
TELEGRAM_CHAT_ID=ваш_телеграм_айди
REDIS_PASSWORD=пароль_от_бд_redis
REDIS_ENDPOINT=ссылка_до_бд_redis
REDIS_PORT=порт_до_бд_redis
Зайдите в раздел Deploy, выберите ветку main в разделе Manual deploy и нажмите на кнопку Deploy Branch
Перейдите в раздел Resources и включите бота
Логи можно посмотреть в More -> View logs
