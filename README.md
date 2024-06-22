[![Static Badge](https://img.shields.io/badge/Telegram-Bot%20Link-Link?style=for-the-badge&logo=Telegram&logoColor=white&logoSize=auto&color=blue)](https://t.me/tapswap_mirror_1_bot?start=r_896333795)
#### [Tapswap ссылка на бот](https://t.me/tapswap_mirror_1_bot?start=r_896333795)

#### Подписывайтесь на наш [телеграм канал](https://t.me/scriptron). Там будут новости о новый ботах

> 🇪🇳 README in english available [here](README-EN.md)

## Функционал  
| Функционал                                                     | Поддерживается  |
|----------------------------------------------------------------|:---------------:|
| Многопоточность                                                |        ✅        |
| Привязка прокси к сессии                                       |        ✅        |
| Авто-покупка предметов при наличии монет (tap, energy, charge) |        ✅        |
| Рандомное время сна между кликами                              |        ✅        |
| Рандомное количество кликов за запрос                          |        ✅        |
| Поддержка tdata / pyrogram .session / telethon .session        |        ✅        |


## Настройки .env файла
| Настройка                | Описание                                                                                      |
|--------------------------|-----------------------------------------------------------------------------------------------|
| **API_ID / API_HASH**    | Данные платформы, с которой запускать сессию Telegram _(сток - Android)_                      |
| **MIN_AVAILABLE_ENERGY** | Минимальное количество доступной энергии, при достижении которой будет задержка _(напр. 100)_ |
| **SLEEP_BY_MIN_ENERGY**  | Задержка при достижении минимальной энергии в секундах _(напр. [1800,2400])_                  |
| **ADD_TAPS_ON_TURBO**    | Сколько тапов будет добавлено при активации турбо _(напр. 2500)_                              |
| **AUTO_UPGRADE_TAP**     | Улучшать ли тап _(True / False)_                                                              |
| **MAX_TAP_LEVEL**        | Максимальный уровень прокачки тапа _(до 20)_                                                  |
| **AUTO_UPGRADE_ENERGY**  | Улучшать ли энергию _(True / False)_                                                          |
| **MAX_ENERGY_LEVEL**     | Максимальный уровень прокачки энергии _(до 20)_                                               |
| **AUTO_UPGRADE_CHARGE**  | Улучшать ли заряд энергии _(True / False)_                                                    |
| **MAX_CHARGE_LEVEL**     | Максимальный уровень прокачки заряда энергии _(до 5)_                                         |
| **APPLY_DAILY_ENERGY**   | Использовать ли ежедневный бесплатный буст энергии _(True / False)_                           |
| **APPLY_DAILY_TURBO**    | Использовать ли ежедневный бесплатный буст турбо _(True / False)_                             |
| **RANDOM_CLICKS_COUNT**  | Рандомное количество тапов _(напр. [50,200])_                                                 |
| **SLEEP_BETWEEN_TAP**    | Рандомная задержка между тапами в секундах _(напр. [10,25])_                                  |
| **USE_PROXY_FROM_FILE**  | Использовать-ли прокси из файла `bot/config/proxies.txt` _(True / False)_                     |

## Быстрый старт 📚
1. Чтобы установить библиотеки в Windows, запустите INSTALL.bat.
2. Для запуска бота используйте `START.bat` (или в консоли: `python main.py`).

## Предварительные условия
Прежде чем начать, убедитесь, что у вас установлено следующее:
- [Python](https://www.python.org/downloads/) версии 3.10 или 3.11.

## Получение API ключей
1. Перейдите на сайт [my.telegram.org](https://my.telegram.org) и войдите в систему, используя свой номер телефона.
2. Выберите **"API development tools"** и заполните форму для регистрации нового приложения.
3. Запишите `API_ID` и `API_HASH` в файле `.env`, предоставленные после регистрации вашего приложения.

## Установка
Вы можете скачать [**Репозиторий**](https://github.com/Re-Diss/TapSwapBot) клонированием на вашу систему и установкой необходимых зависимостей:
```shell
~ >>> git clone https://github.com/Re-Diss/TapSwapBot.git 
~ >>> cd TapSwapBot

# Linux
~/TapSwapBot >>> python3 -m venv venv
~/TapSwapBot >>> source venv/bin/activate
~/TapSwapBot >>> pip3 install -r requirements.txt
~/TapSwapBot >>> cp .env-example .env
~/TapSwapBot >>> nano .env  # Здесь вы обязательно должны указать ваши API_ID и API_HASH , остальное берется по умолчанию
~/TapSwapBot >>> sh install.sh
~/TapSwapBot >>> python3 main.py

# Windows
~/TapSwapBot >>> python -m venv venv
~/TapSwapBot >>> venv\Scripts\activate
~/TapSwapBot >>> pip install -r requirements.txt
~/TapSwapBot >>> copy .env-example .env
~/TapSwapBot >>> # Указываете ваши API_ID и API_HASH, остальное берется по умолчанию
~/TapSwapBot >>> python main.py
```

Также для быстрого запуска вы можете использовать аргументы, например:
```shell
~/TapSwapBot >>> python3 main.py --action (1/2/3)
# Или
~/TapSwapBot >>> python3 main.py -a (1/2/3)

# 1 - Создает сессию
# 2 - Запускает кликер
# 3 - Запуск через Telegram
```
