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
```