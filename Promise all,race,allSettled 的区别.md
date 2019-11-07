```javascript
  var p1 = new Promise((resolve,reject)=>{
    setTimeout(()=>resolve(11),1000)
})


var p2 = new Promise((resolve,reject)=>{
    setTimeout(()=>reject(22),2000)
})



;(async()=>{
    try {
        var p = await Promise.all([p1,p2])
        console.log(p,'<<<<<<all')
    }  catch(e){
        console.log(e,'all')
    }

})()



;(async()=>{
    try{
        var p = await Promise.race([p1,p2])
        console.log(p,'<<<<<<race')
    } catch(e){
        console.log(e,'race')
    }

})()

;(async()=>{
    try{
        var p = await Promise.allSettled([p1,p2])
        console.log(p,'<<<<<<allSettled')
    } catch(e){
        console.log(e,'allSettled')
    }

})()
```
