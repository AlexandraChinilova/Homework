Hello

===========================================

#Tasks from Codewars

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
