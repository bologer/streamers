## 0.0.3 — 22 Февраля 2017

- Добавлена возможность менять цвет темы виджета (светлый или темный)
- CSS корректировки для коректного отображения виджета 
- Возможность изменить тип отображения стримеров (превьюшка самого стрима или его аватарка). Сейчас параметр type принимает два значения — "classic" или "preview"
- Возможность выбрать игру по которой будут показаны стримеры. Делается это теперь параметром `game`
- Изменен каркас виджета, стал более простым и адаптивным
- Увеличена скорость загрузки виджета 
- Исправление ошибок и поправки в коде
- Виджет теперь рабоатет через iframe, чтобы не было проблем с CSS стилями сторонних сайтов

## 0.0.2 — 24 Января 2017

- Возможность поменять язык сайта. Теперь виджет доступен на английском языке. За это отвечает параметр - `streamers_language`, которые принимает значение «ru» или «en».
- Возможность выбрать формат отображения зрителей. С запятой (например: 30,000) или без неё (30000). В разных странах по разному отображаются цифры и поэтому эта функция может пригодиться.
- Возможность показать или скрыть фото автора стрима. Теперь это можно сделать с помощью `displayAuthorPhoto`, который принимает значение «true» или «false»
- Теперь CSS стили для виджета подгружаются всего один раз. До этого был баг с подгрузкой виджета каждый timeout при автоматическом обновлении списка игроков.
- Увеличение скорости загрузки виджета и стабильности работы
- Исправление багов связанных с CSS стилями

## 0.0.1 — 19 Января 2017

- Добавлена возможность вписывать ID своего приложения, чтобы пройти его инициализацию
- Возможность поменять контейнер куда буду вписывать  стримеры
- Возможность поставить лимит на отображение стримеров
- Возможность убрать или поставить анимацию при загрузке стримеров
- Возможность убрать или оставить статуса «LIVE»
- Возможность убрать или оставить флаг стримера
