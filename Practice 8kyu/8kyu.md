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