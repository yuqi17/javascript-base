

```javascript
  var A = [1,2,4]
  var B = [1,2,5,6]
  
  B = B.map(b=>{
     let w = ''
     for(let a of A){
        if(a === b)
        {
          w = 'x';
          break;
        }
        else{
          w = 'y'
        }
     }  
     
     return w;
  })

```
