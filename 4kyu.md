* Square into Squares. Protect trees!
```javascript
function decompose(n) {
console.log(n)
if (n < 4) {return null}
  let arrSq = [];
  let res = [];
  let n2 = n**2;
  let ost = n2;
  for (let i = 1; i**2 < n**2; i++){
   arrSq.push(i**2); 
  }
  arrSq.reverse();
  do {
    for (let a = 0; a < arrSq.length; a++){
     if (arrSq[a] <= ost){
      res.push(arrSq[a]);
      ost -= arrSq[a];
     } 
    }

    if (ost > 0 && ost < 4){
       arrSq.shift(arrSq[0]);
       ost = n2;
       res = [];
    }
   }
  while (ost > 0);
  
  return res.reverse().map((a,i) => a**0.5);
}
```