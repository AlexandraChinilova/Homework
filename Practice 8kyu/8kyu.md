* A Needle in the Haystack
```javascript
function findNeedle(h) {
  for (let i=0; i < h.length; i++){
   if (h[i] === 'needle'){
    return `found the needle at position ${i}`;
   }
  }
}
```
* Sort and Star
```javascript
function twoSort(s) {
  s = s.sort();
  let res = '';
  for (let i=0; i<s[0].length-1; i++){
    res += s[0][i] + '***'
  }
  return res += s[0][s[0].length-1];
}
```
* Abbreviate a Two Word Name
```javascript
function abbrevName(name){
let a = name.split(' ');
 return res = (a[0][0] + '.' + a[1][0]).toUpperCase()
}

//short solution
//return name.split(' ').map(i => i[0].toUpperCase()).join('.')
```
* Get the mean of an array
```javascript
function getAverage(marks){
 return Math.floor((marks.reduce((sum, it) => sum + it))/marks.length)
}
```
* How good are you really?
```javascript
function betterThanAverage(classPoints, yourPoints) {
 let mPoint = (classPoints.reduce((sum,i) => sum+i))/classPoints.length;
 return mPoint <= yourPoints ? true : false;
}
```
* Difference of Volumes of Cuboids
```javascript
function findDifference(a, b) {
  return Math.abs((a[0]*a[1]*a[2]) - (b[0]*b[1]*b[2]))
}
```
* Sum of Multiples
```javascript
function sumMul(n,m){
if (n <= 0 || m <=0){
 return 'INVALID';
}
let sum = 0;
for (let i = n; i< m; i++){
 if (i % n == 0){
 sum += i
 }
}
return sum
}
```
* Grasshopper - Summation
```javascript
function summation(num){
  let i = 1;
  let res = 0;
  while (i <= num){
   res +=i;
   i++;
  }
  return res
}
```
* Count of positives / sum of negatives
```javascript
function countPositivesSumNegatives(input) {
if (input == null || input.length == 0){
return []
}
let count = 0;
let res = [0, 0];
for (let i=0; i<input.length; i++){
 if (input[i] > 0){
  count++
 }
 if (input[i] < 0){
   res[1] += input[i]
   }
}
res[0] = count;
if (res[0] == 0 && res[1] == 0){
 return [];
}
    return res;
}
```
* Invert values
```javascript
function invert(array) {
 return array.map(el => el > 0 ? -el : Math.abs(el))
}
```
* Third Angle of a Triangle
```javascript
function otherAngle(a, b) {
  return 180-(a+b);
}
```
* Generate range of integers
```javascript
function generateRange(min, max, step){
let rez = [];
 for (i = min; i <= max; i = i + step){
  rez.push(i);
 }
return rez
}
```