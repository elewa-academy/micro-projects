## Fun One

Teach someone what this function does, and how it works:

```js
function fun1(){
    var result = [];
    for (var i = 0; i < 5; i++){
        result.push( function() {return i} );
    }
    return result;
}

console.log(fun1()[0]()) 
```

Find an explanation on this [StackOverflow question](https://stackoverflow.com/questions/9069614/javascript-puzzle-scope).

___
___
### <a href="http://elewa.education/blog" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/34921062-506450ae-f97d-11e7-875f-6feeb26ad72d.png" width="100" height="40"/></a>