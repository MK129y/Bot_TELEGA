# Bot_TELEGA
In fil's bot's

After that declaration, we need to register some so-called message handlers. Message handlers define filters which a message must pass. If a message passes the filter, the decorated function is called and the incoming message is passed as an argument.

Let's define a message handler which handles incoming /start and /help commands.
A function which is decorated by a message handler can have an arbitrary name, however, it must have only one parameter (the message).

Edited Message handler
Handle edited messages @bot.edited_message_handler(filters) # <- passes a Message type object to your function

Channel Post handler
Handle channel post messages @bot.channel_post_handler(filters) # <- passes a Message type object to your function

Edited Channel Post handler
Handle edited channel post messages @bot.edited_channel_post_handler(filters) # <- passes a Message type object to your function






























/*
доделать,создать new директорию

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
*/
