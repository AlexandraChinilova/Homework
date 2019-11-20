Hello

===========================================

# Tasks from Codewars

* Function 1 - hello world
```javascript
function greet() {
    return "hello world!";
    }
```
* Remove First and Last Character
```javascript
function removeChar(str){
  let i = 0
  while (i < str.length-1) {
  i++;
}
   str = str.substring(1, i);
  return str;
}
```
* Will you make it?
```javascript
function zeroFuel (s, mpg, g)  {
  if ( s <= mpg * g)return true;
  else return false
}
```
* Capitalization and Mutability
```javascript
function capitalizeWord(word) {
let newWord = word[0].toUpperCase();
for(let i = 1; i < word.length; i++){
newWord += word[i];
}
  return newWord;
}
```
* Type of sum
```javascript
function typeOfSum(a, b) {
  let sum = a + b
  return typeof(sum)
}
```
* If you can't sleep, just count sheep!!
```javascript
function countSheep(num){
  let count = '';
  for (let i = 1; i <= num; i++){
    count += i + ' sheep...';
    }
  return count;
}
```
* Opposite number
```javascript
function opposite(number) {
 return number = - number
}
```
* Convert a string to an array
```javascript
function stringToArray(string){
let newRow = string.split(' ');
return newRow;
}
```
* Determine offspring sex based on genes XX and XY chromosomes
```javascript
// first solution:
function chromosomeCheck(sperm) {
  let resDaughter = "Congratulations! You're going to have a daughter.";
  let resSon = "Congratulations! You're going to have a son.";
  if (sperm === 'XX'){
  return resDaughter;
  } else {
  if (sperm === 'XY'){
  return resSon
}}}

// second solution:
function chromosomeCheck(sperm) {
  return "Congratulations! You're going to have a " + (sperm === 'XX' ? 'daughter' : 'son') + "."
}
```
* Thinkful - Logic Drills: Traffic light
```javascript
function updateLight(current) {
 if (current === 'green'){
 return 'yellow';
 } else {
 if (current === 'yellow'){
 return 'red';
 } else {
 return 'green'
 };
 };
}
```
* The Feast of Many Beasts
```javascript
function feast(beast, dish) {
return (beast[0] == dish[0] && beast[beast.length-1] == dish[dish.length-1]) ? true : false ;
}
```
* Simple multiplication
```javascript
function simpleMultiplication(number) {
let res = 0;
return number % 2 == 0 ? res = number * 8 : res = number * 9;
}
// not mine, but good solution:
function simpleMultiplication(n) {
    return n * (n % 2 ? 9 : 8);
}
```
* Student's Final Grade
```javascript
/// first solution with if:

function finalGrade (exam, projects) {
  if (exam > 90 || projects > 10) {
  return 100;
  } else {
   if (exam > 75 && projects >= 5) {
   return 90;
   } else {
    if (exam > 50 && projects >= 2) {
    return 75;
    } else {
     return 0;
     };
    };
}

// second solution with for:

function finalGrade (exam, projects) {
  for (; exam > 90 || projects > 10; ) {
  return 100;
  }
  for (; exam > 75 && projects >= 5; ) {
   return 90;
  }
  for (; exam > 50 && projects >= 2; ) {
    return 75;
  }
  return 0;
}

// other good solution:
function finalGrade(exam, projects) {
    if (exam > 90 || projects > 10) return 100;
    if (exam > 75 && projects >= 5) return 90;
    if (exam > 50 && projects >= 2) return 75;
    return 0;
}
```
* Reverse a Number
```javascript
// solved together with students
function reverseNumber(n) {
  if (n >= 0) {
  let arr = n.toString().split('').reverse();
    return +(arr.join(''))
    } else {
    n = n * (-1);
    arr = n.toString().split('').reverse();
    return (-1) * (+(arr.join('')))
    }
}
```
* Get list sum recursively
```javascript
// first solution:
function sumR(x) {
if (x.length > 0){
return x.shift() + sumR(x);
} else {
  return 0;
  }
}

// second solution: 
function sumR(x) {
if (x.length === 0){
return 0;
} else {
return x.shift() + sumR(x);
}
}
```
* Reverse List Order
```javascript
function reverseList(list) {
let newList = list.reverse();
return newList
}
```
* Switch it Up!
```javascript
function switchItUp(number){
switch (number) {
  case 0:
    return ( 'Zero');
  case 1:
    return ( 'One' );
  case 2:
    return ( 'Two' );
  case 3:
    return ( 'Three' );
  case 4:
    return ( 'Four' );
  case 5:
    return ( 'Five' );
  case 6:
    return ( 'Six' );
  case 7:
    return ( 'Seven' );
  case 8:
    return ( 'Eight' );
  case 9:
    return ( 'Nine' );
}}

another solution with Julia:
function switchItUp(number){
let arr = ['Zero', 'One', 'Two', 'Tree', 'Four', 'Five', 'Six', 'Seven', 'Eigth', 'Nine'];
 return arr[number];
}
```

* Try to see branch after created.

* Alphabet symmetry
```javascript
function solve(arr){
  let newArr = [];
   for (i = 0; i < arr.length; i++){
    let word = arr[i];
     
function wordCount(word){  
let alfabet   = 'abcdefghijklmnopqrstuvwxyz';
let alfabetUp = 'ABCDEFGHIJKLMNOPQRATUVWXYZ'
let res = 0;
for (j = 0; j < word.length; j++){
  if (alfabet[j] === word[j] || alfabetUp[j] === word[j]){
    res++;
  }
 }
return res;
}
  newArr.push(wordCount(arr[i]));
}
 return newArr;
}
```
* Shortest Word
```javascript
function findShort(s){
let arr = s.split(' ');
let count =[];
  
for (i=0; i < arr.length ; i++) {
  count.push(arr[i].length);
 }
 return Math.min.apply(Math, count)
}
```
* String ends with?
```javascript
function solution(str, ending){
  return (str.slice(-ending.length)===ending)
}
// с применением метода endsWith будет выглядеть так:

function solution(str, ending){
  return str.endsWith(ending);
}
```
* Remove String Spaces
```javascript
function noSpace(x){
let newRow = '';
for ( i=0; i < x.length; i++){
 if (x.charAt(i) !== ' '){
  newRow = newRow + x.charAt(i);
  };
};
return newRow
}

// можно использовать методы:
function noSpace(x){return x.split(' ').join('')}
```
* Do I get a bonus?
```javascript
function bonusTime(salary, bonus) {
return salary10 = '£' + (bonus === true ? salary * 10 : salary);
}
```
* Credit card issuer checking
```javascript
function getIssuer(number) {
iss = String(number);
 if (iss.length == 13 && iss.substring(0,1) == 4 || iss.length == 16 && iss.substring(0,1) == 4){
   return 'VISA'
 }
  if (iss.substring(0,2) == 34 || iss.substring(0,2) == 37 && iss.length == 15){
   return 'AMEX'
  }
   if (iss.substring(0,4) == 6011 && iss.length == 16){
    return 'Discover'
   }
    if (iss.substring(0,2) == 51 ||
        iss.substring(0,2) == 52 ||
        iss.substring(0,2) == 53 ||
        iss.substring(0,2) == 54 ||
        iss.substring(0,2) == 55 && iss.length == 16){
     return 'Mastercard'
    }
    return 'Unknown';
}

// можно с использованием Метода STARTSWITH (чужой вариант):
function getIssuer(number) {
  var card = number.toString();
  if((card.startsWith('34') || card.startsWith('37')) && card.length == 15)
    return 'AMEX';
  else if(card.startsWith('6011') && card.length == 16)
    return 'Discover';
  else if(+card.slice(0,2)>50 && +card.slice(0,2)<56 && card.length==16)
    return 'Mastercard';
  else if(card.startsWith('4') && (card.length==13 || card.length == 16))
    return 'VISA';
  else
    return 'Unknown';
}

// мое измененное решение с учетом нового Метода:
function getIssuer(number) {
iss = String(number);
 if (iss.length == 13 && iss.startsWith('4') || iss.length == 16 && iss.startsWith('4')){
   return 'VISA'
 }
  if (iss.startsWith('34') || iss.startsWith('37') && iss.length == 15){
   return 'AMEX'
  }
   if (iss.substring(0,4) == 6011 && iss.length == 16){
    return 'Discover'
   }
    if (iss.substring(0,2) >=51 && iss.substring(0,2) <= 55 && iss.length == 16){
     return 'Mastercard'
    }
    return 'Unknown';
}
```
* sPoNgEbOb MeMe
```javascript
function spongeMeme(s) {
  let MeMe = '';
   for (i=0; i < s.length; i++){
     if (i % 2 === 0){
       MeMe += s[i].toUpperCase()
     } else {
       MeMe += s[i].toLowerCase()
     }
     }
  return MeMe
}

// another view:
function spongeMeme(s) {
  let MeMe = '';
   for (i=0; i < s.length; i++){
     i % 2 === 0 ? MeMe += s[i].toUpperCase() : MeMe += s[i].toLowerCase();
     }
  return MeMe
}
```
* MakeUpperCase
```javascript
function makeUpperCase(str) {
let res = '';
for (i=0; i < str.length; i++){
 res += str[i].toUpperCase()
 }
  return res;
}
```
* Double Char
```javascript
function doubleChar(str) {
  let double ='';
  for (i=0; i < str.length; i++){
     double += '' + str[i] + str[i]
  }
  return double
}
```

* !!! WeIrD StRiNg CaSe - back to task, level to high - 6
```javascript
function toWeirdCase(s){
  let Weird = s[0].toUpperCase() + '';
   for (i=1; i < s.length; i++){
     if (s[i] == ' ') {
      Weird += s[i];
     } else {
       if (i % 2){
         Weird += s[i].toLowerCase()
       } else {
       Weird += s[i].toUpperCase();
        }
     }}
  return Weird
}

console.log(toWeirdCase('This is a test'));

// 'ThIs Is A TeSt' - must be
// 'ThIs iS A TeSt' - wrong result
```
* String repeat
```javascript
function repeatStr (n, s) {
let res = '';
for (i=0; i < n; i++){
 res += s
 }
  return res;
}
```
* Mumbling
```javascript
function accum(s) {
 let newRow = '';
 let newW = '';
  for (i=0; i < s.length; i++){
   newW = '';
    newW = s[i].repeat(i+1);
    newW = newW.toLowerCase();
    newW = newW[0].toUpperCase() + newW.substring(1);
    if (i === s.length-1){
      newRow += newW + '';
    } else {
   newRow += newW + '-';
   }}
  return newRow
}
```
* Initialize my name
```javascript
function initializeNames(short){
 let arr = short.split(' ');
  let ini = '';
   let newArr = [];
 console.log(arr);
  if (arr.length > 2){
    for (i=1; i < (arr.length-1); i++){
   ini += arr[i].substring(0,1).toUpperCase() + '. '
    }
    ini = arr[0] + ' ' + ini + arr[arr.length-1]
    return ini
  } else {
return newArr = arr.join(' ');
  }
} 

// Обратиться к символу в элементе массива: nameArr[i][0]
// better solution
function initializeNames(name){
  let arr = name.split(' ');
  if (arr.length === 1) return name;
  let str = arr[0] + ' ';
  for (let i = 1; i < arr.length - 1; i++) {
    str += arr[i][0] +'. ';
  }
  str += arr[arr.length-1];
  return str;
}
```
* Array Array Array
```javascript
function explode(x){
 if (typeof x[0] === 'number' && typeof x[1] === 'number'){
   let c = x[0] + x[1];
   return new Array(c).fill(x);
   }
   if (typeof x[0] === 'string' && typeof x[1] === 'number'){
     let d = x[1];
    return new Array(d).fill(x);
   }
  if (typeof x[0] === 'number' && typeof x[1] === 'string'){
     let f = x[0];
    return new Array(f).fill(x);
   }
    if (typeof x[0] === 'string' && typeof x[1] === 'string'){
      return str = 'Void!'
    }
}
```
* Return Negative
```javascript
function makeNegative(num) {
  if (num <= 0) {
   return num
   }
   if (num > 0) {
    return num * -1;
  }
}
```
* Will there be enough space?
```javascript
function enough(cap, on, wait) {
let res = 0;
 if (cap - on > wait){
  return res}
  else { return res = on + wait - cap}
}
```
* Sum Arrays
```javascript
function sum (numbers) {
let a = 0;
 for (i = 0; i < numbers.length; i++){
  a = a + numbers[i];
  }
  return a
}

// Method REDUCE
function sum(numbers) {
  return numbers.reduce((a, b) => a + b, 0);
}
```
* Find out whether the shape is a cube
```javascript
function cubeChecker(volume, side){
  if (volume < 0 || side < 0){
   return false}
    if (volume/(side ** 3) === 1){
     return true}
  return false;
}
```
* Count by X
```javascript
function countBy(x, n) {
  let z = [];
  let a = 0;
 for (i=0; i < n; i++, a += x){
   z.push(a+x);
 }
  return z;
}
```
* Century From Year
```javascript
function century(year) {
 if (year % 100 > 0) {
 return res = Math.floor(year / 100) + 1}
 else {
 return res = Math.floor(year/ 100)}
}
```
* Love vs friendship
```javascript
function wordsToMarks(string){
  let alf = ' abcdefghijklmnopqrstuvwxyz';
   let res = 0;
  for (i=0; i < alf.length; i++){
   for (j=0; j < string.length; j++){
    if (string[j] === alf[i]){
     res += i;
   }}}
  return res
}

// another solution Method charCodeAt()
function wordsToMarks(str)
{
  var sum = 0;
  for (let i = 0; i < str.length; i++)
    sum += str.charCodeAt(i) - 96;
  return sum;
}
```
* Count the Monkeys!
```javascript
function monkeyCount(n) {
let arr = [];
 for (i=1; i <=n; i++){
  arr.push(i);
 }
  return arr
}
```
* Sum of positive
```javascript
function positiveSum(arr) {
 let sum = 0;
  for (i=0; i < arr.length; i++){
   if (arr[i] > 0){
   sum +=arr[i];
   }
  }
  return sum
}

// another solution
function positiveSum(arr) {
      return arr.reduce((a,b)=> a + (b > 0 ? b : 0),0);
   }
```
* Find the divisors!
```javascript
function divisors(n) {
  let arr = [];
   for (i = 2; i < n; i++){
    if (n % i === 0){
     arr.push(i);
    }
   }
      if (arr.length === 0){
       arr = n + ' is prime';
      }
    return arr
};
```
* Returning Strings
```javascript
function greet(name){
  return str = `Hello, ${name} how are you doing today?`;
}
```
* Ordering the words!
```javascript
function orderWord(s){ 
  let arr = [];
  if (s === '' || s === null) {
  return str = 'Invalid String!';
  }
 return arr = s.split('').sort().join('');
}
```
* Bit Counting
```javascript
function countBits(n) {
let str = n.toString(2);
  let count = 0;
  for (i = 0; i < str.length; i++){
   if (str[i] == 1){
    count++
   }
  }
  return count;
}
```
* Convert to Binary
```javascript
function toBinary(n){
  return +n.toString(2);
}
```
* Fake Binary
```javascript
function fakeBin(x){
let res = '';
for (i = 0; i<x.length; i++){
 if (x[i] < 5){
  res += '0';
 } if (x[i] >= 5){
    res += '1';
  }
}
return res;
}
```

* Simple Pig Latin
```javascript
function pigIt(str){
  let arr = str.split(' ');
   for (i = 0; i < arr.length; i++){
     if (arr[i].match(/\w/) !== null && arr[i].match(/\D/) !== null) {
     arr[i] = arr[i].substring(1) + arr[i][0].substring(0,1) + 'ay';
     arr.push();
     }
   }
  return res = arr.join(' ')
}
```
* Arrays Similar
```javascript
function arraysSimilar(arr1, arr2) {
 if (arr1.length == arr2.length){
  arr1.sort();
   arr2.sort();
 for (i=0, j=0; i < arr1.length && j < arr2.length; i++, j++){
   if (arr1[i] === arr2[j]){
   } else {
   return false}
  }
   return true
 }
  return false
}
```
* Remove duplicate words
```javascript
function removeDuplicateWords (s){
  let arr = s.split(' ');
  let nArr = [];
   for (i=0; i < arr.length; i++){
    if (nArr.some(word => word === arr[i]) !== true) {
      nArr.push(arr[i]);
    }
   }
  return newStr = nArr.join(' ')
}
```
* Find the missing element between two arrays
```javascript
function findMissing(arr1, arr2) {
 arr1.sort();
   arr2.sort();
 console.log(arr1, arr2);
  for (i=0; i < arr1.length; i++){
    if (arr1[i] !== arr2[i]){
      return arr1[i]
    }
  }
}
```
* Convert number to reversed array of digits
```javascript
function digitize(n) {
 return res = String(n).split('').reverse().map(Number)
}
// Test.assertDeepEquals(digitize(35231),[1,3,2,5,3]);
```
* Merge two sorted arrays into one
```javascript
function mergeArrays(arr1, arr2) {
 for (i=0; i < arr2.length; i++){
   arr1.push(arr2[i]);
 }
 for (t = 0; t < arr1.length-1; t++){
  for (j=0; j < arr1.length-1; j++){
     if (arr1[j] >= arr1[j+1]){
      let n = arr1[j];
      arr1[j] = arr1[j+1];
      arr1[j+1] = n;
     }
   }
  }
  let nArr = [];
  for (h=0; h < arr1.length; h++){
   if (arr1[h] !== arr1[h+1]){
    nArr.push(arr1[h]);
  }}
  return nArr
}

// another solution
function mergeArrays(arr1, arr2) {
  return Array.from(new Set(arr1.concat(arr2).sort((a,b) => (a-b))));
}
```
* Check the exam
```javascript
function checkExam(a1, a2) {
 let res = 0;
 for (i=0; i < a1.length; i++){
   if (a2[i] === ''){
        continue; }
    if (a1[i] === a2[i]){
      res +=4 ;
    }
     if (a1[i] !== a2[i]){
       res -=1 ;
     }
 }
  if (res < 0){
     return res = 0};
 return res
}
```
* Convert string to camel case
```javascript
function toCamelCase(str){
if (str == ''){
 return str = ''}
 if (str.match(/\-/) == '-'){
  str = str.split('-')}
  else {
  if (str.match(/\_/) == '_') {
   str = str.split('_')}}
for (i=1; i < str.length; i++){
   str[i] = str[i][0].toUpperCase() + str[i].substring(1)
}   
   return str = str.join('')
}

// find symbol in string
```

* Numerical Palindrome #1
```javascript
function palindrome(num) { 
  let str = '';
   if (typeof num !== 'number' || num < 0){
     return 'Not valid'
   }
  str = num + '';
  for (i=0; i < Math.floor(str.length/2); i++){
    if (str[i] !== str[str.length - i - 1]){
     return false;
    }
  }
  return true
} 
// Метод Math.floor() возвращает целое число,
// которое меньше или равно данному числу.

// with methods:
function palindrome(num) { 
   if (typeof num !== 'number' || num < 0){
     return 'Not valid'
   }
  cost arr = +(num.toString().split('').reverse().join('')); 
  
     return num === arr;
} 
```
* Find the calculation type
```javascript
function calcType(a, b, res) {
  if (a + b == res) {
   return 'addition'
  }
  if (a - b == res) {
   return 'subtraction'
  }
  if (a * b == res) {
   return 'multiplication'
  }
  if (a / b == res) {
   return 'division'
  }
}
```

* Simple beads count
```javascript
function countRedBeads(n) {
  return (n - 1) * 2 > 0 ? res = (n - 1) * 2 : 0
}
```
* Array plus array
```javascript
function arrayPlusArray(arr1, arr2) {
let sum = 0;
let arr = arr1.concat(arr2);
 for (i = 0; i < arr.length; i++){
  sum += arr[i] 
 }
  return sum
}
```
* Count Odd Numbers below n
```javascript
function oddCount(n){
if (n % 2){
  return count = (n - 1) / 2;}
  return count = n / 2;
}

// с использованием метода
function oddCount(n){
  return count = Math.floor(n / 2);
}

// зависает при вычислении больших чисел
function oddCount(n){
  let count = 0;
   for (let i = 1; i < n; i++){
    if (i % 2) count++;
   }
  return count
}
```
* Multiples of 3 or 5
```javascript
function solution(number){
  let sum = 0;
   for (i = 1; i < number; i++){
    if (i % 3 === 0 || i % 5 === 0){
     sum += i
    }   
   }
  return sum
}
```
* Sum Mixed Array
```javascript
function sumMix(x){
let sum = 0;
 for (let i = 0; i < x.length; i++){
  if (typeof x[i] == 'string'){
   x[i] = Number(x[i]);
  }
  sum += x[i];
 }
 return sum
}
```
* Who is going to pay for the wall?
```javascript
function whoIsPaying(name){
 let arr = [name];
  if ( name.length > 2){
  arr.push(name.substring(0,2))
  }
  return arr
}
```
* Reverse Vowels In A String
```javascript
function reverseVowels(str) {
  let vowels = ['A','a','E','e','I','i','O','o','U','u'];
  let arrV = [];
  let word = str.split('');
  for (i=0; i < word.length; i++){
    if (vowels.some((item) => word[i] == item)){
      arrV.push(word[i]);
      word[i] = 'time';}
  }
  for (j=0; j < word.length; j++){
      if (word[j] == 'time'){
        word[j] = arrV.splice(-1,1)
      }
    }
return word.join('')
}
```
* Check three and two
```javascript
function checkThreeAndTwo(array) {
  let a = 0;
  let b = 0;
  let c = 0;
  for (let i = 0; i < array.length; i++){
   if (array[i] == 'a'){
    a++
   }
   if (array[i] == 'b'){
    b++
   }
   if (array[i] == 'c'){
    c++
   }
  }
  if (a == 3 && b == 2 || a == 3 && c == 2 || a == 2 && b == 3 || a == 2 && c == 3 || b == 3 && c == 2 || c == 3 && b == 2){
   return true
  }
  return false
}
```
* Remove duplicates from list
```javascript
function distinct(a) {
let res = [a[0]];
for (let i = 1; i < a.length; i++){
 if (res.some(item => item === a[i]) !== true){
  res.push(a[i]);
 }
}
  return res;
}
```
* Even or Odd
```javascript
function even_or_odd(number) {
 return number % 2 ? 'Odd' : 'Even'
}
```
* Smallest Difference
```javascript
function smallestDiff(arr1, arr2) {
  if (arr1.length == 0 && arr2.length == 0){
    return -1
  }
  
  if (arr1.length == 0){
    return Math.min(...arr2)
  }
  if (arr2.length == 0){
      return Math.min(...arr1)
  }
  
  if (arr1.some(item1 => item1 < 0)){
    let min1 = Math.max(...arr1);
    let min2 = Math.min(...arr2);
    return Math.abs(min1 - min2);
  }
  if (arr2.some(item2 => item2 < 0)){
    let min1 = Math.min(...arr1);
    let min2 = Math.max(...arr2);
    return Math.abs(min1 - min2);
  }
  
  if (arr1.some(item1 => item1 < 0) && arr2.some(item2 => item2 < 0)){
    let min1 = Math.max(...arr1);
    let min2 = Math.max(...arr2);
    return Math.abs(min1 - min2);
  }
  let res = [];
   for (let i = 0; i < arr1.length; i++){
    for (let j =0; j < arr2.length; j++){
      res.push(Math.abs(arr1[i]-arr2[j]))
      }
    }
    return Math.min(...res)
}
```
* Lario and Muigi Pipe Problem
```javascript
function pipeFix(numbers){
 let res = [];
 for (let i = numbers[0]; i <= numbers[numbers.length-1]; i++){
   res.push(i)
 }
 return res
}
```
* Mexican Wave
```javascript
function wave(w){
let res = [];
  if (w == '') {
    return res
  }
  let word = w.split('')
  let i = 0;
  while (i < w.length){
    if (word[i] == ' '){
      i++;}
    else {
  word.splice(i,1, word[i].toUpperCase());
  let slovo = word.join('');
  res.push(slovo);
  i++;
   word = w.split('');
   }
}
  return res
}
```
* Print a Rectangle Using Asterisks
```javascript
function getRectangleString(width, height) {
let znak = '*';
let res = '';
 for (let i = 1; i <= height; i++){
   if (i == 1 || i == height){
    res += `${znak.repeat(width)}\r\n`;
  }
  else {
  res += `${znak}${' '.repeat(width-2)}${znak}\r\n`;
  } 
  }
  return res
}
```
* String average
```javascript
function averageString(str) {
  if (str === ''){
  return 'n/a'
  }
  let sum = 0;
  let per = 0;
  let res = 0;
  let arr = str.split(' ');
  for (let i = 0; i < arr.length; i++){
   switch (arr[i]){
     case 'zero' : per = 0;
       break;
     case 'one' : per = 1;
       break;
     case 'two' : per = 2;
       break;
     case 'three' : per = 3;
       break;
     case 'four' : per = 4;
       break;
     case 'five' : per = 5;
       break;
     case 'six' : per = 6;
       break;
     case 'seven' : per = 7;
       break;
     case 'eight' : per = 8;
       break;
     case 'nine' : per = 9;
       break;
     default : return 'n/a'
   }
    sum += per;
  }
  sum = Math.trunc(sum/arr.length);
   switch (sum){
     case 0 : res = 'zero';
       break;
     case 1 : res = 'one';
       break;
     case 2 : res = 'two';
       break;
     case 3 : res = 'three';
       break;
     case 4 : res = 'four';
       break;
     case 5 : res = 'five';
       break;
     case 6 : res = 'six';
       break;
     case 7 : res = 'seven';
       break;
     case 8 : res = 'eight';
       break;
     case 9 : res = 'nine';
       break;
   }
  return res
}

// another solution with object:
function averageString(str) {
  var numObj = {
    'zero': 0,
    'one': 1,
    'two': 2,
    'three': 3,
    'four': 4,
    'five': 5,
    'six': 6,
    'seven': 7,
    'eight': 8,
    'nine': 9
  },
  sum = 0;
  str = str.split(' ');
  for(var i = 0; i < str.length; i++) {
    if(numObj[str[i]] === undefined) {
      return 'n/a';
    } else {
      sum += numObj[str[i]];
    }
  }
  return Object.keys(numObj)[Math.floor(sum/str.length)];
}
```
* Random case
```javascript
function randomCase(x) {
  let res = '';
  for (let i=0; i<x.length; i++){
   if (Math.round(Math.random()) > 0){
    res += x[i].toUpperCase();
   } else {
    res += x[i].toLowerCase();
   }
  }
  return res
}
```
* Simple Simple Simple String Expansion
```javascript
function stringExpansion(s) {
 if (s.match(/\d/g) == null){
       return s;
     }
  let mn = 1;
  let res = '';
  
  if (s[0].match(/\d/) !== null){
    mn = s[0];
   for (let i=0; i<s.length-1; i++){
     if (s[i].match(/\D/) !== null && s[i+1].match(/\D/) !== null){
      res += s[i+1].repeat(mn);
     }
      if (s[i].match(/\D/) !== null && s[i+1].match(/\d/) !== null || s[i].match(/\d/) !== null && s[i+1].match(/\d/) !== null){
      mn = Number(s[i+1]);
      }
       if (s[i].match(/\d/) !== null && s[i+1].match(/\D/) !== null){
      res += s[i+1].repeat(mn);
       }
    }
  } else {
    res = s[0];
    for (let i=0; i<s.length-1; i++){
     if (s[i].match(/\D/) !== null && s[i+1].match(/\D/) !== null){
      res += s[i+1].repeat(mn);
     }
      if (s[i].match(/\D/) !== null && s[i+1].match(/\d/) !== null || s[i].match(/\d/) !== null && s[i+1].match(/\d/) !== null){
      mn = Number(s[i+1]);
      }
       if (s[i].match(/\d/) !== null && s[i+1].match(/\D/) !== null){
      res += s[i+1].repeat(mn);
       }
    }
  }
  return res;
}

//another solution with operator '+'
function stringExpansion(s) {
  let memor = 1;
  let newS = "";
  for (let i = 0; i <s.length; i++){
    if(s[i] == +s[i]){ 
      memor = +s[i];
    }else{
     newS += s[i].repeat(memor);
    }
  }
  return newS;
}
// operator '+' vernet NaN if string  and  number if number!!!
```
* Sort the odd
```javascript
function sortArray(array) {
  if (array.length == 0){
  return array}
  if (array.length > 10){
  for (let i=0; i<array.length; i++){
   if (array[i]%2 > 0){
    delete array[i];
   }
  }
  return array;
  }
  let arrOdd = [];
  for (let i=0; i<array.length; i++){
   if (array[i]%2 > 0 ){
    arrOdd.push(array[i]);
    delete array[i];
   }
  }
  for (let od=0; od < arrOdd.length-1; od++){
   for (let j=0; j<arrOdd.length-1; j++){
    if (arrOdd[j]>arrOdd[j+1]){
     let vr = arrOdd[j];
     arrOdd[j] = arrOdd[j+1];
     arrOdd[j+1] = vr;
    }
   }
  }
  let res = [];
  for (let a=0; a<array.length; a++){
   if (array[a] === undefined){
    res.push(arrOdd.shift())
   } else {
    res.push(array[a]);
     }
  }
  return res;
}
// something wrong with this kata...

// another solution
function sortArray(arr) {
  if(arr.length === 0){
   return [];
  }
   const odd = arr.filter(num => num % 2).sort((a, b) => a - b);
   return arr.map(el => el % 2 ? odd.shift() : el);
}
```
* Create Four Letter Birding Codes from Bird Names
```javascript
function birdCode(arr){
let newArr = [];
for (let i=0; i< arr.length; i++){
 let el = arr[i].replace(/-/g,' ').split(' ');
  if (el.length == 1){
    newArr.push(el[0].slice(0,4).toUpperCase());
  }
  if (el.length == 2){ 
     newArr.push((el[0].slice(0,2) + el[1].slice(0,2)).toUpperCase())
  }
  if (el.length == 3){
    newArr.push((el[0].slice(0,1) + el[1].slice(0,1) + el[2].slice(0,2)).toUpperCase())
  }
  if (el.length >= 4){
    newArr.push((el[0].slice(0,1) + el[1].slice(0,1) + el[2].slice(0,1) + el[3].slice(0,1)).toUpperCase())
  }
}
  return newArr
}
```
* Are the numbers in order?
```javascript
function inAscOrder(arr) {
  for (let i=0; i < arr.length; i++){
   if (arr[i] > arr[i+1]){
     return false
   }
  }
  return true
}
```
* Discover The Original Price
```javascript
function discoverOriginalPrice(dPr, sP){
  return Math.floor((dPr * 100 / (100-sP))*100)/100;
}
//with Method toFixed()
function discoverOriginalPrice(discountedPrice, salePercentage){
  return +(discountedPrice / (1 - salePercentage / 100)).toFixed(2);
}
```
* Clocky Mc Clock-Face
```javascript
function whatTimeIsIt(angle){
  let m = Math.floor(angle*2 % 60);
  let h = Math.floor((angle*2 - m)/60);
    if (h <= 9){h = `0${h}`};
    if (h <= 0) {h = '12'};
    if (m <= 9){m = `0${m}`};
  return `${h}:${m}`
}
```
* Sum of odd numbers
```javascript
function rowSumOddNumbers(n) {
let startN = (n*(n+1))-n*2;
let finishN = n*(n+1);
let res = 0;
	for(let i = startN; i < finishN; i++){
   if (i % 2 !== 0){
   res += i 
   }
  }
  return res
}
// another solution
function rowSumOddNumbers(n) {
  return Math.pow(n, 3);
}
// or
function rowSumOddNumbers(n) {
  return n**3
}
```
* Sum of Odd Cubed Numbers
```javascript
function cubeOdd(arr) {
if (arr.some(item => typeof item !== 'number')){
  return undefined
}
let res = 0;
for (let i=0; i<arr.length; i++){
 arr[i] = arr[i]**3
 if (arr[i] % 2 !== 0){
  res += arr[i]
 }
}
return res
}
```
* Check three and two
```javascript
function checkThreeAndTwo(array) {
let a = 0;
let b = 0;
let c = 0;
  for (let i=0; i<array.length; i++){
  switch (array[i]){
   case 'a' : a++; break
   case 'b' : b++; break
   case 'c' : c++; break
   }
  }
  if (a == 3 && b == 2 || a == 2 && b == 3 || a == 3 && c == 2 || a == 2 && c == 3 || b == 3 && c == 2 || b == 2 && c == 3){
   return true
  }
  return false
}
```
* Two Sum
```javascript
function twoSum(n, t) {
let arr = [];
  for (let i=0; i<n.length; i++){
   for (let j = i+1; j<n.length; j++){
    if ((n[i] + n[j]) == t) {
   arr.push(i);
   arr.push(j);
    }
   }
  }
  return arr
}
```
* Number of People in the Bus
```javascript
function number(p){
let res = 0;
  for (let st = 0; st < p.length; st++){
   res += p[st][0] - p[st][1];
  }
 return res;
 }
 
 // short solution with Methods:
 function number(p){
 return res = p.map(item => item[0]-item[1]).reduce((a,b) => a+b);
  }
```
* Difference Of Squares
```javascript
function differenceOfSquares(n){
  let i=1;
  let sqSum = (n*(n+1)/2)**2;
  let sumSq = 0;
  while (i <= n){
   sumSq += i**2
   i++
  }
  return sqSum - sumSq
}
```
* Bingo Card
```javascript
function getCard() {
 let arr = [];
  let newEl = '';
   for (let i = 0; i < 24; i++){
     if (i < 5){
      do {
       newEl = 'B' + (Math.floor(Math.random()*14)+1)
      } while (arr.some(el => newEl == el))
       arr.push(newEl)
     }
      if (i >=5 && i < 10){
       do {
        newEl = 'I' + (Math.floor(Math.random()*14)+16)
       } while (arr.some(el => newEl == el))
        arr.push(newEl)
      }
       if (i >=10 && i < 14){
        do {
         newEl = 'N' + (Math.floor(Math.random()*14)+31)
        } while (arr.some(el => newEl == el))
         arr.push(newEl)
       }
        if (i >=14 && i < 19){
         do {
          newEl = 'G' + (Math.floor(Math.random()*14)+46)
         } while (arr.some(el => newEl == el))
          arr.push(newEl)
        }
         if (i >=19){
          do {
           newEl = 'O' + (Math.floor(Math.random()*14)+61)
          } while (arr.some(el => newEl == el))
           arr.push(newEl)
         }
   }
   return arr
}
```
* The Supermarket Queue
```javascript
function queueTime(custom, kas) {
 if (custom.length == 0){
  return 0
 }
 if (kas == 1){
  return custom.reduce((a,b) => a+b) 
 }
 if (custom.length <= kas){
  return Math.max(...custom)
 }
 
 const firstLine = custom.splice(0, kas);
 const time = firstLine.slice();
  
 for (let i=0; i < custom.length; i++){
   let minT = Math.min(...firstLine);
   let numKass = firstLine.indexOf(minT);
    for (let f=0; f < firstLine.length; f++){
      firstLine[f] -= minT;
    }
   firstLine[numKass] = custom[i];
   time[numKass] += custom[i];
 }  
  return Math.max(...time)
}
```
* Simple Fun #352: Reagent Formula
```javascript
function isValid(f){
if ((f.some(el7 => el7 === 7)) || (f.some(el8 => el8 === 8))){
   if ((f.some(el1 => el1 === 1)) && (f.some(el2 => el2 === 2)) || (f.some(el3 => el3 === 3)) && (f.some(el4 => el4 === 4))){
   return false
   }
   if ((f.some(el5 => el5 === 5)) && (f.every(el6 => el6 !== 6)) || (f.every(el5 => el5 !== 5)) && (f.some(el6 => el6 === 6))){
   return false
   }
return true
}
return false
}

// with Method includes()
function isValid(f) {
    return (
        !(f.includes(1) && f.includes(2)) &&
        !(f.includes(3) && f.includes(4)) &&
        (f.includes(5) === f.includes(6)) &&
        (f.includes(7) || f.includes(8))
    )
}
```
* Bumps in the Road
```javascript
function bump(x){
let bumps = 0;
for (let i=0; i< x.length; i++){
 if (x[i].match(/n/)) {
  bumps++;
 }
}
return bumps <= 15 ? 'Woohoo!' : 'Car Dead'
}
```
* Sum ALL the arrays!
```javascript
// мое решение, не выполняется для глубоко вложенных массивов на Codewars

function SumNuts(nuts){
 let cup = 0;
  for (let i=0; i<nuts.length; i++){
    if (nuts[i].length == undefined){
      cup +=nuts[i];
    } else {
      cup += SumNuts(nuts[i])
    }
  }
  return cup
}

// другое мое решение

function arraySum(arr){
let sum = 0;
let allNumb = arr.join().split(',');
  for (let i=0; i<allNumb.length; i++){
    if (isNaN(allNumb[i]) == false){
    sum += +allNumb[i]
    }
  }
  return sum
}

// хорошее решение с использованием isArray() и isNaN()

function arraySum(arr) {
  return arr.reduce((n, x) => n + (Array.isArray(x) ? arraySum(x) : isNaN(x) ? 0 : x), 0)
}
```
* Where my anagrams at?
```javascript
function anagrams(word, words){
let res = [];
  
 function countLetters(x){
   let objW = {};
 for (w=0; w < x.length; w++){ 
  if(objW[x[w]] == undefined){
    objW[x[w]] = 1
  } else {
    objW[x[w]]++
  }
 }
  return objW;
 }

let lWord = countLetters(word);

  for (let arr = 0; arr < words.length; arr++){
  if (String(Object.keys(lWord).sort()) === String(Object.keys(countLetters(words[arr])).sort())){
    let count = false;
    for (let key in lWord){
        if (lWord[key] === countLetters(words[arr])[key]){
         count = true
        } else {
          count = false;
          break;
        }
    }
   if (count === true) {
     res.push(words[arr])
   }
  }
}  
  return res
}
```
* Find The Parity Outlier
```javascript
function findOutlier(int){
let a = Math.abs(int[0]%2);
 let b = Math.abs(int[1]%2);
  let c = Math.abs(int[2]%2);
if (a === 0 & a === b || a !== b & a === c & a === 0 || a !== b & b === c & b === 0){
 for (let o=0; o < int.length; o++){
   if (int[o]%2 !== 0){
     return int[o];
   }
 } 
}
  
if (a === 1 & a === b || a !== b & a === c & a === 1 || a !== b & b === c & b === 1){
  for (let e=0; e < int.length; e++){
   if (int[e]%2 === 0){
     return int[e];
   }
 }
}
}
```
* A Gift Well Spent
```javascript
function buy(x, arr){
console.log(x, arr);

if (arr.length === 0 || arr.length < 2 ||
    arr.length === 2 && arr[0] + arr[1] < x){
    return null};
    
let sum2tovar = 0;
let rez = [];
 for (i=0; i < arr.length-1; i++){
  if (arr[i] <= x){
   for (j=i+1; j < arr.length && rez.length == 0; j++){
    sum2tovar = arr[i] + arr[j];
    if (sum2tovar == x){
     rez.push(i);
     rez.push(j);
     return rez;
    }
   }
  }
 }

return null;
};
```
* Perimeter of squares in a rectangle
```javascript
function perimeter(n) {

let sum = [0, 1];
let square = 0
let x = 1;
  for (i=0; i < n; i++){
   square = sum[i]+sum[i+1]
   sum.push(square);
   x = x + square;
  }

return (4 * x);
}
```
* Maximum Triplet Sum (Array Series #7)
```javascript
function maxTriSum(numbers){
  let sum = Math.max(...numbers);
  let maxN = Math.max(...numbers);
   numbers.splice(numbers.indexOf(Math.max(...numbers)), 1);
  for (let i = 0; i < 2;){
    if (Math.max(...numbers) == maxN){
      numbers.splice(numbers.indexOf(Math.max(...numbers)), 1);
    } else {
   sum += Math.max(...numbers);
     maxN = Math.max(...numbers);
   numbers.splice(numbers.indexOf(Math.max(...numbers)), 1);
   i++
    }
  }
  
  return sum
}
```
* Shift Left
```javascript
function shiftLeft(s, t){
 let d = 0;
   while (s != t) {
     if (s.length === 0){
       t = t.slice(1);
       d++;
     }
     if (t.length === 0){
      s = s.slice(1);
      d++;
     }
     if (s.length == t.length){
       s = s.slice(1);
      d++;
       t = t.slice(1);
      d++;
     }
     if (s.length > t.length){
      s = s.slice(1);
      d++;
     }
    if (s.length < t.length){
     t = t.slice(1);
      d++;
    }
  }
  return d
}
```

* Testing 1-2-3
```javascript
function number(array){
  
  for (let i=0; i < array.length; i++){
   array[i] = `${i+1}: ${array[i]}`
  }
  
  return array
}
```
* Phone Directory
```javascript
function phone(strng, num) {

let name = '';
let address = '';
let tel = strng.split('\n');
let person = '';
let countN = 0;
  for (let z=0; z < tel.length; z++){
   for (let i=0; i < tel[z].length; i++){
    if (num == tel[z].substr(i, num.length)){
      countN++;
      person = tel[z];
  name = person.match(/<(.*?)>/)[1]; // /<(.*?)>/ - выводит содержимое между < >.
  person = person.replace(person.match(/<(.*?)>/)[0],'').replace(person.match(num),'').replace(/[,:;+?$/_*&#@!^%]/g, " ");
  // /[:;}%$]/g - можно находить несколько символов сразу используя []
   for (let i=0; i < person.length; i++){
  if (person[i] != ' '){
     address += person[i];
  }
  if (person[i] == ' ' && person[i+1] != ' '){
    address += person[i];
  }
}
        if (countN > 1){
          return `Error => Too many people: ${num}`;
        }
    }
   }
  }
  if (countN == 1){
   address = address.replace(/ /, "");
   if (address[address.length-1] == ' '){
    address = address.slice(0, address.length-1);
   }
    return `Phone => ${num}, Name => ${name}, Address => ${address}`;
  }
  return `Error => Not found: ${num}`;
}
```
