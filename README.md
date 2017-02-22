# Использование виджета

Подключить библиотеку отвечающая за получение и отображение стримеров с [Twitch.tv](https://twitch.tv/).

```html
<script src="//cskatka.ru/api/streamers/js/api.js?1"></script>
```

Далее создать элемент, которые будет отвечать за отображение списка стримеров.

```html
<div id="cskatka-streamers"></div>
```

Теперь вызываем API с минимальными настройками.

```html 
<script>
new CSKatkaSteamers({ 
  appId: ВАШЕ_APP_ID, 
}); 
</script>
```

`appId` — это ID вашего приложения, которые вы получаете после [добавления](http://cskatka.ru/dev/add) вашего сайта в систему. 

> Чтобы получить код для вставки вам нужно [зарегистрироваться](http://cskatka.ru/site/signup) в системе, добавить свой сайт и выбрать нужный вам виджет для вставки на свой сайт. 

Самая простая версия скрипта со всеми стандартными настройками выглядит следующим образом.

```html 
<script src="//cskatka.ru/api/streamers/js/api.js?1"></script>
<div id="cskatka-streamers"></div>
<script>
new CSKatkaSteamers({ 
  appId: ВАШЕ_APP_ID, 
}); 
</script>
```

# Документация 
Всевозможные настройки виджета выглядит следующим образом.

```js
new CSKatkaSteamers({ 
	appId: '',
	container: '#cskatka-streamers', 
	limit: 5, 
	streamer_language: '',
	translate: 'ru',
	type: 'classic',
	theme: 'dark',
	game: 'csgo',
	commaSeparation: true,
	displayAuthorPhoto: true,
	displayFlags: true,
	displayLiveMessage: true,
	displayPreloadingText: true
});
```

| Параметр              | Важный?| Описание                                                                                                                                                        |
|-----------------------|--------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------|
| appId                 | v      | ID вашего сайта                                                                                                                                                 |
| container             |        | Контейнер, которые используется для выведения стримеров. Стандартное значение: `#cskatka-streamers`                                                             |
| limit                 |        | Число выводимых стримеров. Стандартное значение: 5. Минимум — 1 и максимум — 100.                                                                               |
| streamers_language    |        | Выбрать язык стримеров для отображения. Стандартное значение: «ru» (Русский язык). Например, «ru» — рускоговорящие стримеры и «en» для англоговорящих.          |
| translate             |        | Перевод виджета на другой язык. На данный момент доступены следующие языки: ‘ru’ (русский) и ‘en’ (английский). Стадартное значение: «ru» — Русский.            |
| type                  |        | Тип виджета. Классический (classic) — отображается аватар стримера, первью (preview) — отображается обложка самого стрима. Стандартное значение - "classic"     |
| theme					|	     | Тема виджета (темная или светлая). Стандартной значение - "dark". Возможные варианты: "dark" или "white".                                                       |
| game                  |        | Установить по какой игре будут показаны онлайн стримеры. Стандартной значение: "csgo" (Counter Strike: Global Offensive)                                        |
| commaSeparation       |        | Разделять число зрителей запятой или нет. По умолчанию: «true». Где «true» — это число «300000» формируется в «300,000», а при «false» остается первоначальное. |
| displayAuthorPhoto    |        | Отображать фото автора стрима. По умолчанию: «true». Где «true» — да, «false» — нет.                                                                            |
| displayFlags          |        | Отображать флаг страны стримера или нет. По умолчанию: «true». Где «true» — да, «false» — нет.                                                                  |
| displayLiveMessage    |        | Отображать «LIVE» сообщение или нет. По умолчанию: «true». Где «true» — отображать «LIVE» и «false» — нет.                                                      |
| displayPreloadingText |        | Показывать сообщение о загрузке стримеров по типу «Загрузка стримеров..» или нет . По умолчанию: «true» — не показывать, «false» — показывать                   |

## `game` параметр 

Слева в столбце указан возможный вариант значения для `game` параметра. В правом столбце — расшифровка. 

Например, если вы укажите `game: 'csgo'` тогда у вас будут показаны все игры по Counter-Strike: Global Offensive.

| Короткое название | Полное название          | 
|-------------------|--------------------------|
| csgo | Counter-Strike: Global Offensive |
| lol | League of Legends |
| hstone | Hearthstone |
| rus | Rust |
| dota2 | Dota 2 |
| fifa1 | FIFA 17 |
| tshows | Talk Shows |
| kingofkill | H1Z1: King of the Kill |
| overwatch | Overwatch |
| wow | World of Warcraft |
| honor | For Honor |
| creative | Creative |
| minecraft | Minecraft |
| arma3 | Arma 3 |
| poker | Poker |
| clashroyal | Clash Royale |
| worldoftanks | World of Tanks |
| nioh | Nioh |
| tomclancy | Tom Clancy\'s Rainbow Six: Siege |