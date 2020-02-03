WMT - WMT Map Tools

Инструментарий для создания удобных TvT миссий

Дополнительные аддоны WMT [здесь](https://github.com/Zealot111/WMT_MapToolsAdditional)

Подробную справку смотрите [здесь](https://github.com/iEzhuk/WOG3_MapTools/wiki)

v. 1.5 ua - 02.02.2020
* український переклад від Barman75


v. 1.5
* совместимость с ACE
* изменен приоритет вкладки WMT в редакторе
* функция отображения членов экипажа перенесен в модель Main
* удален модель Vehicle
* добавлено возможность выбора победившей стороны по окончанию времени через определение
  функции WMT_fnc_ChooseWinnerByTime, которая должна возвращать массив вида [SIDE, STRING]
* добавлена возможность указывать подкласс CfgDebriefing в параметрах WMT_fnc_EndMissions
* переделан скрипт подсчета потерь
* убрана задержка между удалением ботов и окончанием фризтайма
* вкладка отряда содержит информацию и снаряжении
* приглушение звука по клавише (по-умолчанию: F4)
* 3 пресета для дальности видимости (по-умолчанию: F1, F2, F3)
* отключена возмодность настройки дальности видимости через стандартные настройки
* раздельное настроект дальности видимости для объектов и ландшафта
* изменено меню настроек
* использование cba_fnc_addKeybind для обработки нажатия клавиш
* фикс обратной связи с админом
* измен цвет и кисть  маркера при вызове функции WMT_fnc_BoundingBoxMarker на ColorGrey и SolidFull
* добавлена переменная wmt_feature_frzLegacyActions, при определении которой добавляются
  возможность открытия инвенторя ботов и сохранения бота после фризтайма
* командир отделения может открыть инвентарь бота на фризтайме
* более быстрое обновление информации о голосовании во время фризтайма
* фризтайм продлевается на 1 мин если есть желающие его продолжить и нет желающих стартовать

v. 1.4.4 - 09.04.2015
* фикс отключения чата
* фикс панели связи с администратором
* изменена система генерации частот
* улучшена работа функции WMT_fnc_BriefingMap
* улучшена работа модуля StartPosition
* добавлен сигнал по окончанию фризтайма
* добавлена функция WMT_fnc_CreateGlobalMarker
* добавлено удаление маркеров после окончания фризтайма
* приглушение звука при нахождении в технике

v. 1.4.3 - 04.02.2015
+ поле Condition для модулей задач
+ модуль Compose для композиции задач
+ возможность ограничить список перезаряжаемого вооружения в технике this setVariable ["WMT_Magazines", [...]]
* возвращена генерация частот


v. 1.4.2 - 27.01.2015
* багфиксы удаления ботов
* частоты теперь не генерируются, показываются только дефолтные частоты раций, при этом запись в дневнике появляется только после старта игры, это должно пофиксить баг с невыдачей раций
* через `init.sqf` можно теперь задать `wmt_hl_ratio = [0.1,0.2,0.1];` с долями потерь для каждой из сторон (красная, синяя, зеленая, зеленые считаются синими или красными если в настройках миссии стоят союзниками)

v. 1.4.1 - 27.12.2014
+ добавлен модуль выбора старотовой позиции

v. 1.4.0 - 16.12.2014
* подсветку ника можно выключить на панели настроек
* при опознании тела, никнейм печается на жетончике
* осветительные ракеты освещают теперь гораздо сильнее
* исправлена проблема при подсчете игроков зонах, поставленных через модули
* исправлено толкание лодок, теперь должно работать
* подписка на событие об окончании фризтайма
* выдача карт если у игрока нет карты и он в технике с встроенным gps, около своего боца с картой или в технике со своими  бойцами, экипированными картой
* чат должен выключаться после фризтайма

v. 1.3.6 - 02.12.2014
* не работало переснаряжение техники
* сделан более мелким промежуток цикла проверки времени на фризе

v. 1.3.5 - 25.11.2014
+ интегрирован микромод [STELS]Cowcancry для удаления звуков взрывчатки в WMT_ATFixes.pbo
* время игры теперь стоит во время фриз-тайма
* исправлено, при перазаходе в чужого бота показывался ник того игрока, который заходил в него раньше
* изменен вид показываемого никнейма игрока, никнеймы животных теперь не показываются
* небольшие исправления в текстовых ресурсах
* панель дебага доступна через Home
* боты теперь удаляются при окончании фриз-тайма, у командира отд. есть возможность отменить удаление бота посмотрев на него и выбрав в меню действий "Не удалять бота"

v 1.3.0 - 11.11.2014
+ поддержка изменения длины фризтайма, перевод времени на начальное после конца фризтайма
* изменение имени модуля wmt_vehicle
+ добавлены классы статических паллет Land_Pallet_static_F Land_Pallet_vertical_static_F
+ экранчики катеров показывают не в тепловом режиме а в ночном
+ экранчики MRAP показывают не в тепловом режиме а в дневном

v 1.2.3 - 15.10.2014

+ поддержка телепортации на фризтайме
+ снаряд EP для титанов (классы Titan_AT_Hard 5Rnd_GAT_missiles_hard 1Rnd_GAT_missiles_hard 2Rnd_GAT_missiles_hard)

v 1.2.1 - 13.09.2014

* теперь техника должна нормально переснаряжаться из ящиков или из техники поддержки
+ также перезарядка работает даже если еще остались патроны


v 1.2.0 - 11.09.2014

fixed: орфография
fixed: не работает автоматическая потеря зоны
fixed: не показываемая статистика убийств
fixed: не изменяется дальность видимости в спектаторе
fixed: действие "Капитальный ремонт" отображается даже если поблизости нет спец. техники

changed: более низкий приоритет для стандартного модуля ModuleCreateDiaryRecord_F (запись пудет добавлена после сгенерированных)
changed: в модуле WMT_Time дефолтное значение для удаления ботов с 5 до 3
changed: в модуле WMT_Point дефолтное значение количество игроков для захвата с 0 до 4
changed: в модуле WMT_Point дефолтное значение количество игроков для защиты с 0 до 3
changed: убраны функции из cfgFunction, которые используются только в модулях
changed: генерация брифинга в начале миссии сервером

added: в модуль WMT_Point, добавлен таймер на захват зон
added: в модуль WMT_Point, добавлена возможность составлять зону из нескольких маркеров - "Zone1_1, Zone1_2"
added: синхронизация оставшегося времени со секатором
added: в панель администара добавлено поле "оставшееся время"
added: возможность изменять время миссии через панель администратора (-5, +5, +10 минут)
added: в брифинг добавлена запись "мой отряд"
added: функция WMT_fnc_BriefingMap включающая выдачу карт на брифинг для тех у кого нет карты (необходимо запускать через скрипт)
