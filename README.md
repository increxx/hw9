# Повесть временных лет
Работа выполнена в Sublime Text

__1. Как я удалял пустые строки:__

Сначала я удалил пустые строки, используя регулярное выражение : ^\n

<img width="1440" alt="1" src="https://user-images.githubusercontent.com/35449941/41207762-cf4e2ccc-6d23-11e8-8ddb-db9d33aec3e7.png">

Через некоторое время я обнаружил в тексте другие пустые строки с пробелами. Чтобы от них избавиться, я использовал следующее регулярное выражение : ^\s

<img width="1440" alt="2" src="https://user-images.githubusercontent.com/35449941/41207763-cf6f4a38-6d23-11e8-9bc7-a3c4dad54e57.png">

__2. Как я искал всех князей и города, имя и название которых оканчивается на "слав"...:__

Чтобы найти все имена собственные, оканчивавшиеся на -слав, я пользовался регулярным выражением:
[А-Я][а-яѣ]+слав[а-яѣ]+

Всего упоминаний: 564

Так, в строке 49 можно заметить, что слово "славу" не выделилось.

<img width="1440" alt="3" src="https://user-images.githubusercontent.com/35449941/41207764-cf8cf7ae-6d23-11e8-8b0b-ecc04be034d3.png">

__3. Упоминания Новгорода:__

Здесь использовал регулярное выражение: Нов.город+[^.?!;:-]

Всего упоминаний Новгорода найдено: 58

<img width="1440" alt="123" src="https://user-images.githubusercontent.com/35449941/41207765-cfab346c-6d23-11e8-86d3-56acda5705cc.png">

__4. Бонус__

Здесь я применял следующее регулярное выражение: ([!,.;:"?-])

Также я заменил на: $1 (пробел)

<img width="1440" alt="bonus" src="https://user-images.githubusercontent.com/35449941/41207766-cfc71a9c-6d23-11e8-8d6c-17ec5af94cd6.png">
