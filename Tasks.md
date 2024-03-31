# Объемные задачи

## Задачи


### React

[Среднее время](https://codesandbox.io/s/stupefied-cache-sepkql).        
[Получение данных](https://codesandbox.io/s/eager-gianmarco-xdvo9h).   
[Timer](https://codesandbox.io/s/timer-react-17-forked-8903ot?file=/src/timer.tsx) - [решение](https://codesandbox.io/s/timer-react-17-forked-v3o6e6?file=/src/timer.tsx)

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
```
type GetID<ITEM> = (item: ITEM) => string

/**
 * Исключает item из массива, если элемент есть в массиве, иначе добавляет item в конец массива
 * Возвращает новый массив
 *
 * @param item элемент массива
 * @param array массив
 * @param getId возвращает id элемента, нужен для поиска элемента в массиве
 */
export const toggleItem = <ITEM>(item: ITEM, array: ITEM[], getId: GetID<ITEM>): ITEM[] => {
  return []
}
```
```
interface TreeData {
  id: string
  value: number
  children?: TreeData[]
}

interface FlatData extends Omit<TreeData, 'children'> {
  parent?: FlatData['id']
}

/**
 * Преобразование древовидной структуры TreeData в плоскую FlatData
 *
 * @param tree Древовидная Структура
 */

 export const toFlatData = (tree: TreeData): FlatData[] => {

}
```
```
interface SplitResult {
  left: number[]
  inner: number[]
  right: number[]
}

/**
 * Разбивает массив чисел points на 3 части по условию:
 * left: числа меньше всех чисел из periods
 * right: числа  больше всех чисел из periods
 * inner: оставшиеся числа
 *
 * Пример:
 * const points = [-1, 0, 12, 1, 5]
 * const periods = [3, 2, 5]
 *
 * splitByPeriod(points, periods)
 * > { left: [-1, 0, 1], inner: [5], right: [12] }
 *
 * @param points массив точек
 * @param periods массив периода
 */
```
```
// EX. 1
// DESCRIPTIONS: Type result of console.log instead of '?'

const arr = [1,2,3];
const arr2 = [...arr];

//console.log(arr); // [12, 1, 2, 3]
//console.log(arr2); // [12, 1, 2, 3, 14]
```

```
// EX. 2
// DESCRIPTION: Type the order of numbers which will be printed in the console

// setTimeout(() => {
//    console.log(1);
// });

// const p = new Promise((resolve) => {
//    console.log(2);
//   resolve();
// });

// p.then(() => {
//    console.log(3);
// })

//  console.log(4);
```

```
// EX. 3
// DESCRIPTION: Make expressions work
// RULE: do not change console.log 

// console.log((1).plus(2).minus(1) === 2); 
// expected result: true

// Array.prototype.repeater
// console.log([1,2,3,4,5].repeater(4)); 
// expected result: [1,2,3,4,5,1,2,3,4,5,1,2,3,4,5,1,2,3,4,5]
```

```
// EX. 4
// DESCRIPTION: flat an array

// const flat = (arr) => {
//   // TODO: implement
// }

// console.log(flat([0, 1, [2, [3, [4, 5], 6], [7, 8]], 9]));
// expected result: [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
```
```
// EX. 5
// DESCRIPTION: makes items of an array unique

// const uniq = (arr) => {
// };

// console.log(uniq([ 1, 2, 45, 3, 2, 1, 3, 2, 1, 45, 5 ]));
//expected result: [ 1, 2, 45, 3, 5 ]
```

```
// EX. 6
// DESCRIPTION: a simple memo function
// RULES: unlimited number of args but each of them is primitive

// const memo = (fn) => {
//   // TODO: implement
// };

// const sum = memo((a, b) => a + b);

// console.log('1 + 2 = ' + sum(1, 2)); // expected result: 1 + 2 = 3
// console.log('2 + 3 = ' + sum(2, 3)); // expected result: 2 + 3 = 5
// console.log('cache', sum.cache); // should display cache values
```
```
// Ex. 7
// DESCRIPTION: find pairs of numbers in an array
// RULE: no duplicates

// const getPairs = (arr, ref) => {
//   const newArr
// }

// console.log(getPairs([1, 0, 13, -4, 8, 12, -19, 5, 32], 13));
// expected result: [[1, 12], [0, 13], [8, 5], [-19, 32]]
```
```
// EX. 8
// DESCRIPTION: Implement a function which allows to filter an array with any depth, by filter function

// const deepFilter = (arr, filterFn) => {
//   // TODO: implement
// };

// const filterFunc = (val) => {
//   // TODO: implement
// }

// console.log(deepFilter([null, ['abc', -1, 5, true], -1, 3, [false], [-5, [6, '']]], filterFunc);
// result: [['abc', 5, true], 3, [[6]]]
```


