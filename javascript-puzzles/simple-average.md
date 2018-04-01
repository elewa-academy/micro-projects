## Simple Average

De-tangle this one:


```
'use strict'

function simpleAverage () {
  const averager = {
    avg: 0.0,
    count: 0
  }

  averager.reset = function reset () {
    averager.avg = 0.0
    averager.count = 0
    return averager
  }

  averager.add = function add (samples) {
    [].concat(samples).forEach(function (sample) {
      ++averager.count
      averager.avg += (sample - averager.avg) / averager.count
    })
    return averager
  }

  return averager
}

module.exports = simpleAverage
```js

Read this project [on GitHub](https://github.com/Kikobeats/simple-average/).


___
___
### <a href="http://elewa.education/blog" target="_blank"><img src="https://user-images.githubusercontent.com/18554853/34921062-506450ae-f97d-11e7-875f-6feeb26ad72d.png" width="100" height="40"/></a>