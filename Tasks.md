# Объемные задачи

## Задачи


### React

[Среднее время](https://codesandbox.io/s/stupefied-cache-sepkql).        
[Получение данных](https://codesandbox.io/s/eager-gianmarco-xdvo9h)
[Timer](https://codesandbox.io/s/timer-react-17-forked-8903ot?file=/src/timer.tsx)

### [buildQueryString](https://ru.hexlet.io/challenges/js_collections_query_string_exercise)

```
Реализуйте и экспортируйте функцию по умолчанию, которая принимает на вход список параметров и возвращает сформированный query string из этих параметров:
import bqs from ‘../buildQueryString.js’;
bqs({ per: 10, page: 1 });
// page=1&per=10
Имена параметров в выходной строке должны располагаться в алфавитном порядке (то есть их нужно отсортировать)
```

### [summaryRanges](https://ru.hexlet.io/challenges/js_arrays_summary_ranges_exercise)

```
Реализуйте и экспортируйте по умолчанию функцию, которая находит в массиве непрерывные возрастающие последовательности чисел и возвращает массив с их перечислением.
Примеры
summaryRanges([]);
// []
summaryRanges([1]);
// []
summaryRanges([1, 2, 3]);
// [‘1->3’]
summaryRanges([0, 1, 2, 4, 5, 7]);
// [‘0->2’, ‘4->5’]
summaryRanges([110, 111, 112, 111, -5, -4, -2, -3, -4, -5]);
// [‘110->112’, ‘-5->-4’]
```

### [formattedTime](https://ru.hexlet.io/challenges/intro_to_programming_time_exercise)

```
Реализуйте и экспортируйте по умолчанию функцию, которая принимает на вход количество минут (прошедших с начала суток) и возвращает строку, являющуюся временем в формате чч:мм. Если количество минут содержит больше 24 часов (1 суток), то функция возвращает время, прошедшее с полуночи последних суток.
Примеры:
formattedTime(5); // 00:05
formattedTime(15); // 00:15
formattedTime(60); // 01:00
formattedTime(67); // 01:07
formattedTime(175); // 02:55
formattedTime(600); // 10:00
formattedTime(754); // 12:34
formattedTime(1504); // 01:04
Подсказки
Используйте функцию Math.floor(number) для округления до нижней границы.
```

### [sameParityFilter](https://ru.hexlet.io/challenges/js_functions_same_parity_exercise)

```
Реализуйте и экспортируйте по умолчанию функцию, которая принимает на вход массив и возвращает новый, состоящий из элементов, у которых такая же чётность, как и у первого элемента входного массива.
Примеры
sameParity([-1, 0, 1, -3, 10, -2]); // [-1, 1, -3]
sameParity([2, 0, 1, -3, 10, -2]); // [2, 0, 10, -2]
sameParity([]); // []
```

### [flatten](https://ru.hexlet.io/challenges/js_trees_flatten_exercise)

```
Реализуйте и экспортируйте по умолчанию функцию, которая делает плоским вложенный массив.
Для решения задачи нельзя использовать готовые методы для выравнивания массивов.
Примеры
const list = [1, 2, [3, 5], [[4, 3], 2]];
flatten(list); // [1, 2, 3, 5, 4, 3, 2]
Подсказки
Array.isArray - проверяет, является ли элемент массивом.
```

### [promisify](https://ru.hexlet.io/challenges/js_asynchronous_programming_promisify_exercise)

```
promisify.js
Реализуйте и экспортируйте по умолчанию функцию, которая “промисифицирует” асинхронные функции с колбеками.
import promisify from ‘../promisify.js’;
const readFile = promisify(fs.readFile);
const writeFile = promisify(fs.writeFile);
const filepath = ‘/tmp/myfile’;
writeFile(filepath, ‘content’)
  .then(() => readFile(filepath))
  .then(console.log);
Реализация этой функции опирается на тот факт, что колбек в асинхронных функциях всегда передается последним параметром.
Подсказка
Вам понадобятся rest и spread операторы
```








