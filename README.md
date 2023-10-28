# План подготовки к собеседованию

## Просмотр видео-собеседование

вебдев [веб-дев](https://www.youtube.com/watch?v=ycYp7CYOnO0&list=PLNkWIWHIRwMFSLI9wBuHxuGI5lAZ7QNUg&index=3).  
hr-позвонит [hr-позвонит](https://www.youtube.com/results?search_query=hr+%D0%BF%D0%BE%D0%B7%D0%B2%D0%BE%D0%BD%D0%B8%D1%82)  
Подготовка к собеседованию по JavaScript в
2021.[Подготовка к собеседованию по JavaScript в 2021.](https://www.youtube.com/watch?v=H5wnkRJBfA8).

## Сайты тренажеры

[js-тренажор](https://github.com/lydiahallie/javascript-questions)     
[Набор задач](https://bigfrontend.dev/).   
[Набор алгосов по js](https://leetcode.com/problemset/javascript/).   

## Решение задач/практика

codewars
freecodecamp // ES6,  
Regular Expressions/  
Debugging/  
Basic Data Structures/  
Basic Algorithm Scripting/  
Object Oriented Programming/
Functional Programming/  
Intermediate Algorithm Scripting/  
JavaScript Algorithms and Data Structures Projects

## Книги

YDKJS - get started v2 на русском  
YDKJS - scopes and closures   
YDKJS - про приведение типов

## Статьи

[Ликбез из тачилы ](https://www.youtube.com/playlist?list=PLcvhF2Wqh7DMGR08yA6oNKJ7WCM0tGd4z)  
[Собес Дена Абрамова](https://www.youtube.com/watch?v=XEt09iK8IXs&t=647s)  
[Как работает JavaScript: массивы и хэш-таблицы](https://nuancesprog.ru/p/14613/)  
[Front-end. Вопросы на собеседовании](https://github.com/YauhenKavalchuk/interview-questions)
[300+ ВОПРОСОВ ПО JAVASCRIPT НА СОБЕСЕДОВАНИИ](https://itvdn.com/ru/blog/article/300-js)    
[70 ВОПРОСОВ ПО JAVASCRIPT НА СОБЕСЕДОВАНИИ](https://habr.com/ru/post/486820/)    
[35 ВОПРОСОВ ПО JAVASCRIPT НА СОБЕСЕДОВАНИИ](https://habr.com/ru/post/578370/)    
[Яндекс-фронтенд](https://www.youtube.com/c/%D0%A4%D1%80%D0%BE%D0%BD%D1%82%D0%B5%D0%BD%D0%B4/videos)    
[33 Concepts Every JavaScript Developer Should Know](https://github.com/leonardomso/33-js-concepts).

1) [Как парсит браузер](https://webdevblog.ru/kak-brauzer-renderit-veb-stranicu/)  , [вторая статья как работает браузер](https://habr.com/ru/post/484900/)
2) Вопросы по css
3) [Прото и прототипы](https://www.youtube.com/watch?v=b55hiUlhAzI&list=RDCMUCTW0FUhT0m-Bqg2trTbSs0g&start_radio=1&t=3s)
4) Конструктор и this.
5) [SOLID](https://www.youtube.com/watch?v=WMO9aarO390&list=PLz_dGYmQRrr8rWKkoB3BtxF7JpCzUKny_)
6) http/https
7) crud + хедеры
8) Оптимизации + кеши
9) [Более подробно евентлуп-1](https://www.youtube.com/watch?v=6XyifyzmSMM&t=1s)
10) [Еще евентлуп](https://www.youtube.com/watch?v=qz6yDqjMVfw&t=1s)
11) DNS
12) [Паттерны](https://www.youtube.com/watch?v=bTiAfLbmsnY&t=3s)
13) [Preload,Preconnect,Prefetch](https://nitropack.io/blog/post/resource-hints-performance-optimization)
14) [Жизненный цикл](https://julesblom.com/writing/react-hook-component-timeline?ck_subscriber_id=1866528443&utm_source=convertkit&utm_medium=email&utm_campaign=%E2%9A%9B%EF%B8%8F+This+Week+In+React+%23124%3A+FLIP,+Lifecycle,+Next.js,+TypeScript,+Vanilla-Extract,+LiveView,+Remix,+GitHub,+Race+Conditions,+Fontpie,+Remotion...%20-%209416696)
15) [Reconsiciliatiom](https://www.youtube.com/watch?v=NPXJnKytER4&t=24s)
## Алгосы

[grind75](https://www.techinterviewhandbook.org/grind75)
[Качаем литкод](https://www.linkedin.com/feed/update/urn:li:activity:7001142282578010112/)

# Собеседование

**5 минут** Приветствие, small talk, план собеседования

- Предупредить, что буду делать записи
- Могу прервать, если не будет хватать времени

**10 минут** Расскажите о себе ()

- о своем опыте
- об ожиданиях и желаемой роли, 
- самая сложная задача или серьезный факап  
- что изучили за последнее время 

**15 минут** Live coding

**15 минут**  Теория по JS, TS

**15 минут**  Frameworks - React / State managers / CSS in JS / Webpack / Mfe

**20 минут**  ООП, дизайн принципы и паттерны, Rest, GraphQL, способы интеграции, тестирование, troubleshooting, CI/CD,
leadership

**5 минут** Церемонии в скрам, как проходит эстимация + ретроспектива от кандидата

**5 минут** Вопросы от кандидата

### Задачи на собес

#### Проверка на палиндром

A palindrome is a word, phrase, number, or other sequence of characters which reads the same backward as forward.
Examples of numerical palindromes are:   
2332  
110011   
54322345   
For a given number num, write a function to test if it's a numerical palindrome or not and return a boolean (true if it
is and false if not).
Return "Not valid" if the input is not an integer or less than 0.

//Решение

```js
function palindrome(num) {
    if (typeof num !== 'number' || num < 0) return 'Not valid'
    return String(num).split('').reverse().join('') === String(num)
}
```

#### Проверка на наличие дубликатов

Given an integer array nums, return true if any value appears at least twice in the array, and return false if every
element is distinct.

//Решение

```js
const containsDuplicate = (nums) => {
    return new Set(nums).size !== nums.length
};
```

## React задачи

[Среднее время](https://codesandbox.io/s/stupefied-cache-sepkql).    
[Получение данных](https://codesandbox.io/s/immutable-sun-xge1y1?file=/src/App.tsx).  
[Найти баг](https://codesandbox.io/s/epic-swanson-2dmp2x).  
[yandex-code](https://code.yandex-team.ru)
### JS + TS

Какие существуют типы данных в JS?    
Как проверить, является ли объект массивом?    
Что такое деструктуризация?    
Чем JS отличается при работе на front-end и back-end?    
Для чего предназначены методы setTimeout и setInterval, есть ли они в JS?    
Сравните подходы работы с асинхронным кодом: callbacks vs promises vs async / await.         
Назовите методы массивов, какие помните, и скажите, для чего они нужны.    
Map и Set.     
Глубокая (deep) и поверхностная (shallow) копия объекта.     
Какая разница между декларацией функции (function declaration) и функциональным выражением (function expression)? Что такое анонимная функция?    
Отличия стрелочных функций от обычных:     
IIFE (Immediately Invoked Function Expression).   
Hoisting.    
Замыкание (closure).   
Рекурсия.   
Разница между методами call и apply      
Garbage Collector (сборщик мусора).   
Promise.   
Преимущества генераторов:     
Чистая функция.   
Event Loop (евент-петля)     
RAF.   
Прототип в JavaScript.     
Generics.   
Разница между any и unknown.    
Type guard.   
Type vs Interface.    
Utility типы.   

Partial<T> - создает тип, который делает все свойства объекта необязательными.
Readonly<T> - создает тип, который делает все свойства объекта доступными только для чтения.
Record<K, T> - создает тип, который определяет объект с ключами типа K и значениями типа T.
Pick<T, K> - создает тип, который выбирает только определенные свойства из объекта T на основе типов K.
Omit<T, K> - создает тип, который удаляет определенные свойства из объекта T на основе типов K.


### React / State manager

- Ознакомлены ли вы с хуками? В чем их преимущества? Приходилось ли делать свои и с какой целью?
- Знакомы ли вы с фрагментами и порталами? Зачем они нужны?
- Когда и для чего используют рефы?
- В чем разница useRef и useState?
- Какие вы знаете методы жизненного цикла компонента?
- В каком методе жизненного цикла компонента лучше делать запросы на сервер? Почему?
- В каком методе жизненного цикла компонента лучше делать подписку и отписку от листенера? Почему? Зачем отписываться?
- Был ли опыт работы с контекстом? Когда его стоит использовать
- В чем особенность PureComponent?
- В чем видите преимущества библиотеки React?
- Что такое Virtual DOM и Shadow DOM?
- Зачем в списках ключи? Можно ли делать ключами индексы элементов массива? Когда это оправдано?
- Приходилось ли вам настраивать проект React с нуля? С помощью каких инструментов вы это делали?
- Что самое сложное вам приходилось реализовывать с помощью React?

### Common

- Как обрабатываются ошибки? В каком случае можно перезаписать return в функции?
- Какие методики отпимизации приложения и метрики вы знаете?
- Что вы знаете про доступность?
- Как клиент взаимодействует с сервером? - socket/rest/graphql/sse/long poling 
- Что значит HTTP?
- Какие методы HTTP-запросов вы знаете?
- Какая разница HTTP vs HTTPS?
- Какие знаете коды ответа (состояния) HTTP?
- Что такое CORS?
- Что такое cookie?
- Что такое REST?
- Объяснить понятие мутабельность/иммутабельность? Какие типы являются мутабельными и наоборот?
- Как искать ошибки в коде? Используете ли вы дебаггер?
- Назовите способы хранения данных в браузере.
- Какие паттерны знаете и используете в работе?
- Что такое ci/cd
- Для чего нужен package-lock.json?
- Можете ли вы описать суть методологии git flow/Trunk Based в двух словах?
- SOLID
- WebWorkers
- ServiceWorkers
- SSR/SSG/CSR/SPA/PWA
- Что такое микросервисы?
- Что знаете про тестирование? Какие типы тестов есть? Что такое пирамида тестирования? Как и что тестируете?   
  Подходы: {
    - TDD -это методология разработки ПО, которая основывается на повторении коротких циклов разработки:
      изначально пишется тест, покрывающий желаемое изменение, затем пишется программный код,
      который реализует желаемое поведение системы и позволит пройти написанный тест.
      Затем проводится рефакторинг написанного кода с постоянной проверкой прохождения тестов.
    - BDD — behaviour-driven development — это разработка, основанная на описании поведения.
      Определенный человек(или люди) пишет описания вида "я как пользователь хочу когда нажали кнопку пуск
      тогда показывалось меню как на картинке" (там есть специально выделенные ключевые слова).
      Программисты давно написали специальные тулы, которые подобные описания переводят в тесты (иногда совсем прозрачно
      для
      программиста). А дальше классическая разработка с тестами.

    - DDD - это набор принципов и схем, направленных на создание оптимальных систем объектов.
      Процесс разработки сводится к созданию программных абстракций, которые называются моделями предметных областей.
      В эти модели входит бизнес-логика, устанавливающая связь между реальными условиями области применения продукта и
      кодом.
      }
- С чего начинается создание фичи/компонента/проекта
- Как выбирать библиотеки?
