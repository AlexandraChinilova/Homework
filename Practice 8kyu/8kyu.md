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
*
```javascript
function howMuchILoveYou(l) {
   
  switch (l%6){
   case 1 : return "I love you";
   case 2 : return "a little";
   case 3 : return "a lot";
   case 4 : return "passionately";
   case 5 : return "madly";
   case 0 : return "not at all";
  } 
   
}
```
* Draw stairs
```javascript
function drawStairs(n) {
 if (n == 1) {
 return 'I'
 } 

  let i = 1;
  let stair = '';
  while (i < n){
  stair += 'I\n';
    for (let p = 0; p < i; p++){
      stair += ' '
    }
    i++;
  }
  stair += 'I'
  return stair
}
```
* Sum of differences in array
```javascript
function sumOfDifferences(arr) {
arr.sort((a,b) => b - a);
let sum = 0;
for (let i = 0; i < arr.length-1; i++){
 sum += (arr[i] - arr[i+1]);
}
 return sum
}
```
* Keep up the hoop
```javascript
function hoopCount (n) {
  if (n >= 10){return 'Great, now move on to tricks'}
  return 'Keep at it until you get it'
}
```
* Complementary DNA
```javascript
function DNAStrand(dna){
  let res = '';
   for (let i=0; i < dna.length; i++){
    if (dna[i] === 'A') res += 'T';
    if (dna[i] === 'T') res += 'A';
    if (dna[i] === 'G') res += 'C';
    if (dna[i] === 'C') res += 'G';
   }
  
  return res
}
```
* Keep Hydrated!
```javascript
function litres(time) {
  return Math.floor(time * 0.5);
}
```
* Counting sheep...
```javascript
function countSheeps(arrayOfSheep) {
  let res = 0;
   for (let i=0; i < arrayOfSheep.length; i++){
     if (arrayOfSheep[i] == true){
       res += 1;
     }
  }
  return res
}
```
* Grasshopper - Personalized Message
```javascript
function greet (name, owner) {
 if (name == owner){
  return 'Hello boss'
 }
 return 'Hello guest'
}
```
* Plus - minus - plus - plus - ... - Count
```javascript
function catchSignChange(arr){
let r = 0;
 for (let i=0; i < arr.length; i++){
  if (arr[i] >= 0 && arr[i+1] < 0 || arr[i] < 0 && arr[i+1] >= 0){
   r++;
  }
 }
 return r
}
```