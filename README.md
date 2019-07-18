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