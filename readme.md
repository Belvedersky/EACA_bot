# 🤖 [Бот ВК](https://glitch.com/~belvedersky-eaca-bot) 
* бот работает на [glitch](glitch.com/~belvedersky-eaca-bot)
* будить тут [eaca-bot.glitch.me](belvedersky-eaca-bot.glitch.me ) 
* писать боту сюда [vk.com/eaca_memes](https://vk.com/eaca_memes)
___
## Умеет сейчас
1. Отправлять расписание по комманде [/расписание](src/Commands/ScheduleCommand.js) [группа]
```
/расписание 425
```

```
День: Вторник
⏱ 13:00 - 14:35
История У.П. Ефремова Ауд. 103

⏱ 14:45 - 16:20
Теория и практика коммуникаций И.А. Ахьямова Ауд. 103
```
2. Cоздавать изображение с текстом по комманде [/написать](src/Commands/Text2Image.js) [текст]
```
/написать Lorem Ipsum - это текст-"рыба", часто используемый в печати и вэб-дизайне. Lorem Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI века. В то время некий безымянный печатник создал большую коллекцию размеров и форм шрифтов, используя Lorem Ipsum для распечатки образцов. Lorem Ipsum не только успешно пережил без заметных изменений пять веков, но и перешагнул в электронный дизайн.
```

![Reply](https://pp.userapi.com/c854028/v854028700/38293/uRY2MWXDDlI.jpg)
___

## TODO
* Надо разобраться с получением четности недели и днем недели.
* Не получается отправить длинный текст, проблема в парсинге запроса или что то ограничивает получение изображения.
* Сделать нормальную авторизацию, сейчас идет авторизация easyvk потом объект vk.session.access_token передается bots а там опять в easyvk 😬.
* Прикрутить простенькую базу типо sqlite и хранить там настройки пользователей.
___
## Использованные библиотеки

#### Для работы с VK
> * [Easy VK](https://ciricc.github.io) Надстройка над api vk
> * [vk-bots](https://github.com/ciricc/vk-bots) Надстройка над easyvk )))

#### Для работы с текстом и изображениями
> * [text2png](https://github.com/tkrkt/text2png) Создание изображения из текста
> * [word-wrap](https://github.com/jonschlinkert/word-wrap) Для переноса строки

#### Общего назначения
> * [node-fetch](https://github.com/bitinn/node-fetch) Запросы
> * [underscore](http://underscorejs.ru) Утилиты
> * [date-fns](https://github.com/date-fns/date-fns) Время/Дата

