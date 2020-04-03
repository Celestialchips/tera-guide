# tera-guide
A generic guide module for TERA with English and Russian translations (detects automaticly). Supports of all actual dungeons.

Модуль подсказок по данжам TERA (вывод подсказок в чат и отрисовка зон атак боссов и механик), русская локализация. Поддерживаются все актуальные данжи.

## Зависимости / Dependencies
https://github.com/tera-toolbox-mods/library

Распаковать в директорию "mods" в вашей Tera-Proxy. НЕ РАСПАКОВЫВАТЬ КАК "library-master", ДИРЕКТОРИЯ ДОЛЖНА НАЗЫВАТЬСЯ "library".

Extract to "mods" directory in your Tera-Proxy. DO NOT INSTALLED IT AS "library-master" MAKE SURE IT'S NAMED "library".

## Команды / Commands
Toolbox(/8) | Описание команды<br>Command Description
--- | ---
guide | - вкл./выкл. модуля (по-умолчанию: включено)<br> - on/off, default system notification, notification color yellow
guide alert | - вкл./выкл. сообщений в чате (по-умолчанию: включено)<br> - chat notice on/off
guide systemNotice | - вкл./выкл. сообщений в группе (по-умолчанию: выключено)<br> - party chat notice on/off
guide spawnObject | - вкл./выкл. спавна объектов (по-умолчанию: включено)<br> - spawn area marker objects on/off
guide stream | - вкл./выкл. режима скрытия сообщений (по-умолчанию: включено)<br> - streamer mode (hide all messages and objects) on/off
guide dungeons | - список всех поддерживаемых данжей и их id<br> - list of all supported dungeons and its ids
guide verbose `id` | - вкл./выкл. всех сообщений для данжа, где `id` - идентификатор данжа<br> - messaging for specified by `id` dungeon on/off
guide spawnObject `id` | - вкл./выкл. спавна объектов для данжа, где `id` - идентификатор данжа<br> - spawn area marker objects for specified by `id` dungeon on/off
guide help | - вывод поддерживаемых команд<br> - list of supported commands

## Поддерживаемые данжи / Supported Dungeons
id | Dungeon Name | Название данжа
--- | --- | ---
9067 | Demokron Factory (Hard) | Лаборатория Берна (сложно)*
9970 | Ruinous Manor (Hard) | Руины Кошмарной Абнукты*
9781 | Velik's Sanctuary | Святилище Велики
9981 | Velik's Sanctuary (Hard) | Разрушенное Святилище Велики
9735 | RK-9 Kennel | Ангар RK-9
9935 | RK-9 Kennel (Hard) | Ангар совершенного RK-9*
9720 | Antaroth's Abyss | Омут Антароса*
9920 | Antaroth's Abyss (Hard) | Омут Бездушного Антароса
9782 | Grotto of Lost Souls | Мастерская Леандра*
9982 | Grotto of Lost Souls (Hard) | Заброшенная мастерская Леандра
9044 | Bahaar's Sanctum | Святилище Бахаара
3101 | Gossamer Vault | Гнездо Паркин*
3201 | Gossamer Vault (Hard) | Гнездо сверкающей Паркин
3023 | Akalath Quarantine | Секретное подземелье крепости Берарк
3020 | Sea of Honor | Золотая чешуя
3026 | Corrupted Skynest | Логово Келсаика
3126 | Corrupted Skynest (Hard) | Логово Бессмертного Келсаика
3027 | Forbidden Arena | Арена безумия

&#x002A; - закрыты на RU с обновлением от 8 апреля.

## Misc
Based on https://github.com/michengs/tera-guide and https://github.com/tera-mod/TERA-Guide-Area

More info available on project wiki https://github.com/hsdn/tera-guide/wiki
