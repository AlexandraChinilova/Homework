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