# Things.

That is, some hints, things, and playing with github.

---

## path-array.php

See [path-array.php](path-array.php)

PathArray class - enables working on 'dot notation'  like:
```
$exampleInputData = ['user' => ['name' => 'John', 'sex' => 'male'] ];
echo PathArray::get($exampleInputData, 'user.name');// (We can use different separators than '.')
```

Working example: https://3v4l.org/kYeN9


## typed-array.php 

See [typed-array.php](typed-array.php)

TypedArray class - A very simple implementation of 'typed array', like this:

```
$stringArray = new TypedArray('string');
and now only strings can be added to the above $stringArray. Works with objects as well.
```

More examples below the class.

Ah, and here is a working example: https://3v4l.org/kHocv (can be outdated though)


## check-stuff.php

See [check-stuff.php](check-stuff.php)

Overcomplicated script checking your PHP's error logging configuration.
just copy and paste the above code to some file and run it.


## code-benchmark.php

See [code-benchmark.php](code-benchmark.php)

Returns an execution time in microseconds (one millionth (0.000001 or 1/1,000,000) of a second). 

Example: this should take about 4 seconds, because we repeat it 2 times: 
```
echo benchmark (function(){
    sleep(1);
    sleep(1);
}, 2);
```

## error-reporting.md

See [error-reporting.md](error-reporting.md)

How to make PHP errors/warning to log/display

## named-parameters.php

See [named-parameters.php](named-parameters.php)

"Named parameters" in PHP. There is no such thing, but we can "simulate" it with arrays.

In Python we can do:
```
def info(x = 1, y = 2, z = 3):
and then call it like this:
info(x = 100)
```
We can't do that in PHP, but we can simply pass an array with key => value pairs.

This is a working code - https://3v4l.org/Yj8vT

## var-dump-str.php

See [var-dump-str.php](var-dump-str.php)

var_dump returning a string, in case we need it, for example to log it to a file, example:

``` 
error_log("Something something: ", var_dump_str($someArray)); 
```
Working example: https://3v4l.org/BGCgH
