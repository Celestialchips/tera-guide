# tera-guide
The dungeon guide module with Text-to-speech notifications, display hints on screen and drawing zones of bosses attacks and mechanics. Available English and Russian languages (detects automatically).

Модуль подсказок по данжам с возможностью голосовых уведомлений, вывод подсказок в чат или на экран, а также отрисовка зон атак боссов и механик. Поддерживаются Русский и Английский языки (определяются автоматически).

&#x1F534; **A critical updates have been released. Please update!  
&#x1F534; Были выпущены критические обновления. Пожалуйста, обновитесь!**

* Versión en español del módulo (Spanish translation): https://github.com/Loliconera/tera-guide-spanish
* Versão em português do módulo (Portuguese translation): https://github.com/emilia-s2/Guia-DG-Portugues

## Dependencies / Зависимости
* **tera-guide-core** - https://github.com/hsdn/tera-guide-core

When using TeraToolbox, all dependencies will be installed automatically.   
При использовании TeraToolbox, все зависимости будут установлены автоматически.

## Commands / Команды
Toolbox(/8) | Command description | Описание команды
--- | --- | ---
**guide** | Module on/off | Вкл./выкл. модуля
**guide&nbsp;gui** | Show module GUI| Показать графический интерфейс
**guide&nbsp;voice**<br>(default: on) | Text-to-speech (TTS) notices on/off, speech rate is set by command **guide `1`~`10`** | Вкл./выкл. голосовых уведомлений (TTS), скорость чтения задается командой **guide `1`~`10`**
**guide&nbsp;lNotice**<br>(default: off) | Send notices to chat channel "Notice" instead of on-screen messages on/off | Вкл./выкл. отправки уведомлений в канал чата "Важно" вместо показа экранных сообщений
**guide&nbsp;gNotice**<br>(default: off) | Send notices to party chat channel on/off | Вкл./выкл. отправки уведомлений в канал чата группы
**guide&nbsp;`1`~`10`**<br>(default: 2) | Set TTS speech rate | Регулировка скорости чтения голосовых сообщений
**guide&nbsp;spawnObject**<br>(default: on) | Spawn marker objects on/off | Вкл./выкл. спавна маркировочных объектов
**guide&nbsp;stream**<br>(default: off) | Streamer Mode on/off (hide all notices and objects, TTS will played) | Вкл./выкл. режима стримера (скрывает все уведомления и маркеры, TTS будет проигрываться)
**guide&nbsp;dungeons** | List of all supported dungeons and its ids | Список всех поддерживаемых данжей и их id
**guide&nbsp;verbose&nbsp;`id`**<br>(default: on for all) | Send notices for specified by `id` dungeon on/off | Вкл./выкл. всех уведомлений для данжа, где `id` - идентификатор данжа
**guide&nbsp;spawnObject&nbsp;`id`**<br>(default: on for all) | Spawn marker objects for specified by `id` dungeon on/off | Вкл./выкл. спавна объектов для данжа, где `id` - идентификатор данжа
**guide&nbsp;help** | List of supported commands | Вывод поддерживаемых команд

## Supported dungeons / Поддерживаемые данжи
id | Dungeon name | Название данжа
--- | --- | ---
9781 | Velik's Sanctuary | Святилище Велики
9739 | Red Refuge | Лагерь повстанцев
9735 | RK-9 Kennel | Ангар RK-9
3034 | Rampaging RK-9 Kennel | Ангар RK-9 (сложно)
9920 | Antaroth's Abyss (Hard) | Омут Бездушного Антароса
9982 | Grotto of Lost Souls (Hard) | Заброшенная мастерская Леандра
9044 | Bahaar's Sanctum | Святилище Бахаара
3201 | Gossamer Vault (Hard) | Гнездо сверкающей Паркин
3023 | Akalath Quarantine | Секретное подземелье крепости Берарк
3020 | Sea of Honor | Золотая чешуя
3026 | Corrupted Skynest | Логово Келсаика
3126 | Corrupted Skynest (Hard) | Логово Бессмертного Келсаика
3102 | Draakon Arena | Командный центр
3202 | Draakon Arena (Hard) | Командный центр (сложно)
3027 | Forbidden Arena [Hagufna] | [Бессмертный воин] Арена безумия
3103 | Forbidden Arena [Undying Warlord] | [Этерния] Арена безумия
3203 | Forbidden Arena [Nightmare Undying Warlord] | [Бессмертный] Арена безумия
9053 | Kezzel's Gorge (5-Person) | Ущелье Кеззела (5 игроков)

## Notices settings / Настройка уведомлений

* On screen (on bottom side) and chat notices, if **lNotice** parameter is *on*.   
  Уведомления на экране (в нижней части), а также в чате, если параметр **lNotice** - *включен*.   
  ![](https://i.imgur.com/BPlK58M.png)

* When **gNotice** parameter is *on*, notices will also be sent to party chat channel.   
  Если параметр **gNotice** был *включен*, уведомления также будут отправляться в канал чата группы.   

* The message on top side of the screen, if **lNotice** parameter is *off* (by default).   
  Сообщение в верхней части экрана, если параметр **lNotice** - *выключен* (по-умолчанию).   
  ![](https://i.imgur.com/r2bb8Wc.png)   
  You can set the color for this type of notices using the commands or GUI (also change color in the Toolbox chat).   
  Возможен выбор цвета для этого вида уведомлений при помощи команд или графического интерфейса (также изменяется цвет в чате Toolbox).

* When Streamer Mode is *on* (**stream** parameter), all text notices ONLY sent to Toolbox(/8) chat channel, but TTS notices will be played.   
  Если *включен* режим стримера (парам. **stream**), все текстовые уведомления будут отправляться ТОЛЬКО в канал чата Toolbox(/8), однако голосовые уведомления будут проигрываться.

* To disable or enable TTS notifications, use the **guide voice** command.   
  Для отключения или включения голосовых уведомлений используется команда **guide voice**.

## Module GUI / Графический интерфейс

* When you enter the **guide gui** command, the module GUI is displayed, allowing you to change basic settings.   
  При вводе команды **guide gui** отображается графический интерфейс модуля, позволяющий осуществить основные настройки.   
  ![](https://i.imgur.com/7zAeYhi.png)

## Development and Debugging / Разработка и отладка
Подробнее на https://github.com/hsdn/tera-guide/wiki

## Credits
- **[Kasea](https://github.com/tera-toolbox-mods)** - Original developer of Tera-Guide module
- **[michengs](https://github.com/michengs)** - Author of base code for most guides and module core
- **[ZC](https://github.com/tera-mod)** - Provided coordinates for rendering attack areas and mechanics
- **[Kuroine](https://github.com/Kuroine)** - Author of base code for the DA guide
- **[Multarix](https://github.com/Multarix)** - Author of the RR guide and also making changes to the English translation
- **[Owyn](https://github.com/Owyn)** - Developer of great guides for RK-9, AA and GV, whose code was used
- **[ITunk](https://github.com/GrafNikola)** - Author of initial Russian translation
- **[Loliconera](https://github.com/Loliconera)** - Author of Spanish translation
- **[Emilia](https://github.com/emilia-s2)** - Author of Portuguese translation
