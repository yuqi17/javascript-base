

```javascript


  var A = [1,2,4]
  var B = [1,2,5,6]
  
  for(let a of A){
    for(let b of B){
      if(a === b)
      {
        b = 'x'
        break;
      }
      else{
        b = 'y'
      }
        
    }
  }

```
