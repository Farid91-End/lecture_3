
# Java Script Lecture_3
## 1. Что такое Methods в JS
## 2. STRING
## 3. Number 

### Что такое Methods в JS

В JavaScript методы представляют собой функции, связанные с объектами, которые выполняют определенные действия. Они используются для манипуляции данными и изменения состояния объектов. Методы в JavaScript являются свойствами объектов и могут вызываться с использованием точечной нотации.

##### Создание методов:

Для создания метода нужно добавить функцию в качестве свойства объекта. Вот пример:

    const объект = {
      свойство: значение,
      метод: function() {
        // код метода
      }
    };

##### Вызов метода: 
- Для вызова метода используется точечная нотация, где после имени объекта указывается имя метода и круглые скобки. **Вот пример:**



       объект.метод();

В этом примере мы вызываем метод **метод** у объекта **объект**.

#####Передача аргументов в методы:
Методы могут принимать аргументы, аналогично обычным функциям. Аргументы передаются в круглых скобках при вызове метода. **Вот пример:**

    const объект = {
      свойство: значение,
      метод: function(аргумент1, аргумент2) {
        // код метода
      }
    };

    объект.метод(значение1, значение2);

В этом примере мы передаем **значение1** и **значение2** в метод **метод** у объекта **объект**.

####Возвращаемые значения:
Методы могут также возвращать значения. Для этого используется оператор **return** внутри метода. **Вот пример**:

    const объект = {
      свойство: значение,
      метод: function() {
        // код метода
        return результат;
      }
    };

    const результат = объект.метод();

В этом примере мы сохраняем возвращаемое значение метода **метод** в переменной **результат**.


### Что такое string и методы String в JS
- Строка (String) - это тип данных в JavaScript, который представляет текстовую информацию. Строки в JavaScript заключаются в одинарные или двойные кавычки, например: "Привет, мир!" или 'Hello, world!'.

JavaScript предоставляет ряд методов (встроенных функций), которые могут быть применены к строкам. Вот некоторые из наиболее распространенных методов String в JavaScript:

1. **length**: Возвращает длину строки (количество символов).

        const str = "Hello, world!";
        const length = str.length; // 13

2. **toUpperCase()**: Преобразует все символы строки в верхний регистр.

        const str = "Hello, world!";
        const uppercaseStr = str.toUpperCase(); // "HELLO, WORLD!"

3. **toLowerCase()**: Преобразует все символы строки в нижний регистр.

        const str = "Hello, world!";
        const lowercaseStr = str.toLowerCase(); // "hello, world!"

4. **charAt(index)**: Возвращает символ в строке, находящийся по указанному индексу.

        const str = "Hello, world!";
        const char = str.charAt(7); // "w"

5. **substring(startIndex, endIndex)**: Возвращает подстроку, начиная с индекса **startIndex** до индекса **endIndex** (не включая его).

        const str = "Hello, world!";
        const substring = str.substring(7, 12); // "world"


6. **split(separator)**: Разделяет строку на массив подстрок, используя указанный разделитель.

        const str = "Hello, world!";
        const words = str.split(" "); // ["Hello,", "world!"]
  
7. **indexOf(substring)**: Возвращает индекс первого вхождения подстроки **substring** в строку. Если подстрока не найдена, возвращается -1.

        const str = "Hello, world!";
        const index = str.indexOf("world"); // 7

8. **replace(searchValue, replaceValue)**: Заменяет все вхождения **searchValue** в строке на **replaceValue**.

        const str = "Hello, world!";
        const newStr = str.replace("world", "John"); // "Hello, Farid!"

9. **startsWith(substring)**: Проверяет, начинается ли строка с указанной подстроки **substring**. Возвращает **true** или **false**.

        const str = "Hello, world!";
        const startsWithHello = str.startsWith("Hello"); // true

10. **endsWith(substring)**: Проверяет, заканчивается ли строка указанной подстрокой **substring**. Возвращает **true** или **false**.

        const str = "Hello, world!";
        const endsWithWorld = str.endsWith("world!"); // true

11. **includes(substring)**: Проверяет, содержит ли строка указанную подстроку **substring**. Возвращает **true** или **false**.

        const str = "Hello, world!";
        const includesWorld = str.includes("world"); // true

12. **trim()**: Удаляет пробельные символы в начале и конце строки.

        const str = "   Hello, world!   ";
        const trimmedStr = str.trim(); // "Hello, world!"


13. **charAt(index)**: Возвращает символ в строке по указанному индексу.

        const str = "Hello, world!";
        const char = str.charAt(4); // "o"

14. **concat(string2, string3, ...)**: Объединяет строки, добавляя их к исходной строке.

        const str1 = "Hello";
        const str2 = "world";
        const str3 = str1.concat(", ", str2, "!"); // "Hello, world!"

15. **slice(startIndex, endIndex)**: Возвращает часть строки, начиная с индекса **startIndex** и до индекса **endIndex** (не включая его).

        const str = "Hello, world!";
        const slicedStr = str.slice(7, 12); // "world"

16. **repeat(count)**: Создает и возвращает новую строку, повторяя исходную строку count раз.

        const str = "Hello";
        const repeatedStr = str.repeat(3); // "HelloHelloHello"

17. **match(regexp)**: Ищет совпадения строки с заданным регулярным выражением **regexp** и возвращает массив с найденными совпадениями.

        const str = "Hello, World!";
        const matches = str.match(/o/g); // ["o", "o"]

18. **search(regexp)**: Ищет совпадение строки с заданным регулярным выражением **regexp** и возвращает индекс первого совпадения.

        const str = "Hello, World!";
        const index = str.search(/o/g); // 4

19. **padStart(targetLength, padString)**: Дополняет строку слева с использованием заданной подстроки **padString**, чтобы достичь целевой длины **targetLength**.

        const str = "Hello";
        const paddedStr = str.padStart(10, "x"); // "xxxxxHello"

20. **padEnd(targetLength, padString)**: Дополняет строку справа с использованием заданной подстроки **padString**, чтобы достичь целевой длины **targetLength**.

        const str = "Hello";
        const paddedStr = str.padEnd(10, "x"); // "Helloxxxxx"


Это лишь некоторые из множества методов, доступных для работы со строками в JavaScript. Используйте их в соответствии с вашими потребностями для обработки и манипуляции строковыми данными.

##Методы Number в JS

Вот несколько методов, доступных для работы с числами (Number) в JavaScript:

1. `toFixed(numDigits)`: Преобразует число в строку, округляя его до указанного числа десятичных знаков (numDigits) и возвращает строковое представление числа.
```javascript
const number = 3.14159;
const fixedNumber = number.toFixed(2); // "3.14"
```

2. `toString(radix)`: Возвращает строковое представление числа в указанной системе счисления (radix). По умолчанию, если radix не указан, используется десятичная система счисления.
```javascript
const number = 42;
const binaryString = number.toString(2); // "101010"
```

3. `toPrecision(precision)`: Преобразует число в строку с указанной точностью (precision) и возвращает строковое представление числа. Учитывает как целую, так и десятичную части числа.
```javascript
const number = 3.14159;
const preciseNumber = number.toPrecision(4); // "3.142"
```

4. `parseInt(string, radix)`: Преобразует строку (string) в целое число с указанной системой счисления (radix) и возвращает полученное число.
```javascript
const string = "42";
const parsedNumber = parseInt(string); // 42
```

5. `parseFloat(string)`: Преобразует строку (string) в число с плавающей запятой и возвращает полученное число.
```javascript
const string = "3.14";
const parsedNumber = parseFloat(string); // 3.14
```

6. `isNaN(value)`: Проверяет, является ли значение (value) NaN (Not-a-Number), и возвращает `true` или `false`.
```javascript
const number = NaN;
const isNotANumber = isNaN(number); // true
```

7. `isFinite(value)`: Проверяет, является ли значение (value) конечным числом (не NaN, Infinity или -Infinity), и возвращает `true` или `false`.
```javascript
const number = 42;
const isFiniteNumber = isFinite(number); // true
```

8. `toFixed()`, `toString()`, `toPrecision()`, `parseInt()`, и `parseFloat()` также являются методами объектов типа Number.
```javascript
const number = new Number(42);
const stringNumber = number.toString(); // "42"
```

##Методы объекта Math()
Вот некоторые из методов объекта Math, предоставляемого JavaScript для выполнения математических операций:

1. `Math.abs(x)`: Возвращает абсолютное значение числа `x`.
```javascript
const number = -5;
const absoluteValue = Math.abs(number); // 5
```

2. `Math.ceil(x)`: Возвращает наименьшее целое число, которое больше или равно числу `x`.
```javascript
const number = 4.2;
const ceilValue = Math.ceil(number); // 5
```

3. `Math.floor(x)`: Возвращает наибольшее целое число, которое меньше или равно числу `x`.
```javascript
const number = 4.8;
const floorValue = Math.floor(number); // 4
```

4. `Math.round(x)`: Возвращает ближайшее целое число к числу `x`.
```javascript
const number = 4.5;
const roundedValue = Math.round(number); // 5
```

5. `Math.max(x1, x2, ..., xn)`: Возвращает наибольшее значение из заданных чисел `x1`, `x2`, ..., `xn`.
```javascript
const maxNumber = Math.max(10, 5, 8, 12); // 12
```

6. `Math.min(x1, x2, ..., xn)`: Возвращает наименьшее значение из заданных чисел `x1`, `x2`, ..., `xn`.
```javascript
const minNumber = Math.min(10, 5, 8, 12); // 5
```

7. `Math.pow(x, y)`: Возвращает значение числа `x`, возведенное в степень `y`.
```javascript
const power = Math.pow(2, 3); // 8
```

8. `Math.sqrt(x)`: Возвращает квадратный корень числа `x`.
```javascript
const squareRoot = Math.sqrt(25); // 5
```

9. `Math.random()`: Возвращает псевдослучайное число в диапазоне от 0 (включительно) до 1 (исключительно).
```javascript
const randomValue = Math.random(); // случайное число между 0 и 1
```

Это лишь несколько из множества методов объекта Math, доступных в JavaScript. Они помогают выполнять различные математические операции и вычисления.









