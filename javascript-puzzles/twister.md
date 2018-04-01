## Twister

Teach someone what this function does, and how it works:

```js
function outer(_name) {
	function inner(name) {
		return outer(name);
	};
	inner.title = _name;
	inner.twist = function(name) {
		return this(name);
	};
	return inner;
};
```


___
___
### <a href="http://elewa.education/blog" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/34921062-506450ae-f97d-11e7-875f-6feeb26ad72d.png" width="100" height="40"/></a>