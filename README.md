# ExChat - Новый плагин на чат для вашего сервера!

Что представляет из себя плагин?
- Плагин может заменить вам любые плагины на чаты, ведь он вмещает в себе все что нужно для вашего сервера,
- Как пример наш плагин может менять вид чата лишь по одной команде!

В чем его остальные особености?
- Изменение вида чата по команде;
- Поддержа градиента;
- Легкая настройка;
- Обьяснение что и как в конфиге;
- Очистка чата;
- Сохранение чата;
- Блокировка запрещенных слов;
- Колдаун для каждой группы;
- Вид чата для каждой группы;
- Глобальный и локальный чат;

# Необходимые плагины для работы ExChat
- LuckPerms [Скачать](https://luckperms.net/download).
- PlaceholderAPI [Скачать](https://www.spigotmc.org/resources/placeholderapi.6245/).

# Плагины которые поддерживает ExChat
- DiscordSRV [Скачать](https://www.spigotmc.org/resources/discordsrv.18494/).

# Почему вы должны скачать ExChat?
- Он абсолютно не нагружает сервер, очень понятен в настройке и вмещает в себе все нужное;

# Конфигурация плагина:
```
# # # # # # # # # # # # # # # # # # # # # # # # #
#                                               #
#         Плагин студии ExStudio                #
#             Заказать плагин:                  #
#     https://t.me/exstudio_minecraft           #
#                                               #
# # # # # # # # # # # # # # # # # # # # # # # # #

# Создатели плагина: froriym, coilwer
# Дата создания плагина: 07.08.2024
# Плагин имеет поддержку DiscordSRV
# Необходимые плагины для работы ExChat:
# LuckPerms, PlaceholderAPI
# Все права плагина и их приоритеты:
# exchat.chat1 - op, exchat.chat2 - op, exchat.chat3 - op
# exchat.set - op, exchat.color - op, exchat.chat - op
# exchat.local - op, exchat.global - op, exchat.bypassfilter - op
# exchat.bypasscooldown - op, exchat.reload - op
# все команды плагина:
# /exchat set <вид чата>, /exchat chat clear, exchat chat save <кол-во> /exchat reload
# удачного использования!

chats:
  chat1:
    enabled: true # доступен ли чат в игре для выбора: true - доступен / false - недоступен
    permission: "exchat.chat1" # права на установку чата
    format: '&7<%player%>: %message%' # формат чата
  chat2:
    enabled: true
    permission: "exchat.chat2"
    format: '&7[%player%]: %message%'
  chat3:
    enabled: true
    permission: "exchat.chat3"
    format: '&7{%player%}: %message%'

local: # локальный чат
  enabled: true # доступен ли чат в игре: true - доступен / false - недоступен
  radius: 50 # радиус чата (в блоках)
  format: '&7[&eL&7] %message%' # формат локального чата
  permission: "exchat.local" # права на использование локального чата

global: # глобальный чат
  enabled: true
  format: '&7[&6G&7] %message%'
  prefix: "!"
  permission: "exchat.global"

permissions:
  color: # цветной чат в (через &)
    enabled: true # доступен ли в игре
    permission: "exchat.color" # права на использование цветного чата

group-formats: # виды чата для каждой группы по умолчанию (Требуется LuckPerms)
  default: chat1 # default - группа / chat1 - вид чата
  vip: chat2
  premium: chat3

filters: # фильтр запрещенных слов
  blocked-words-enabled: true # радотает ли в игре, true - работает / false - не работает
  blocked-words:
    - "запрещенное1" # список запрещщеных слов
    - "запрещенное2"
  block-links: true # блокировка ссылок в чате
  block-ips: true # блокировка айпи в чате

cooldowns: # колдаун на использование чата (Подержка LuckPerms)
  enabled: true # радотает ли в игре, true - работает / false - не работает
  default: 5 # в секундах
  vip: 3
  premium: 1
```

