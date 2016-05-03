#### lpawslambda
#####
```
var event={key1:'val1',key2:'val2'};

var context={
  succeed:function(event){
    console.log('succ');
    console.log(JSON.stringify(event,null,2));
  },
  fail:function(event){
    console.log('fail');
    console.log(JSON.stringify(event,null,2));
  },
  done:function(event){
    console.log(JSON.stringify(event,null,2));
  }
};

handler(event,context);
```
