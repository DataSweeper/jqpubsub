**JQuery pub sub pattern example**

Subscripe to to a topic

```
test = function(a) {
  console.log(a)
}

test0 = function() {
  console.log('test0')
}

$.subscribe('test', test)
$.subscribe('test', test0)

$.publish('test', ["a"])

output:
  a
  test0

$.unsubscribe(['test', test0])

$.publish('test', ["a"])

output:
  a
```

