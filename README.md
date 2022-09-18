# Equivalence in languages

## Array -> string 
```php
Input -> v = ["S", "t", "r", "i", "n", "g"]

Python : "".join(v)
JavaScript : v.join("")
PHP : implode("", v)
Java : String.join("", v)

Output -> "String"
```

## String -> array 
```php
Input -> v = "String"

Python : list(v)
JavaScript : v.split("")
PHP : str_split(v) / explode(" ", v) if separator != ""
Java : v.split("")

Output -> ["S", "t", "r", "i", "n", "g"]
```

## Array of lower case letters
```php
Python : list(string.ascii_lowercase)
JavaScript : String.fromCharCode(...Array(123).keys()).slice(97).split("")
PHP : range('a', 'z')
Java : 

Output -> ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']
```

## Array of upper case letters
```php
Python : list(string.ascii_uppercase)
JavaScript : String.fromCharCode(...Array(91).keys()).slice(65).split("")
PHP : range('A', 'Z')
Java : 

Output -> ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
```

## Repeat a string
```php
Input -> v = "String", a = 3

Python : v*a
JavaScript : v.repeat(a)
PHP : str_repeat(v, a)
Java : v.repeat(a)

Output -> "StringStringString"
```

|v : variable| Python | JavaScript | PHP | Java |
| --- | --- | --- | --- |--- |
| type of v | type(v) |  | | v.getClass().getSimpleName() |
| array to string | "".join(v) | v.join("") | implode("", v) | String.join("", v) |
| string to array | list(v) | v.split("") | explode("", v)/str_split(v) | v.split("") |
| add in array | arr.append(v) | arr.push(v) | $arr[] = v | |
| reverse string | v[::-1] | v.split("").reverse().join("") | strrev(v) |  |
| reverse array | v[::-1] | v.reverse() | array_reverse(v) |  |
| show v | print(v) | console.log(v) | echo v/print_r(v) |System.out.println(v) |
| sort array | v.sort(key=len, reverse=False) | v.sort() | sort(v)/rsort(v) | |
| numerical value | int(v) | parseInt(v) | intval(v) | Integer.parseInt(v) |
| string value | str(v) | v.toString() | strval(v) | String.valueOf(v) |
| replace value in str | | | | v.replace('a) |
| sqrt | math.sqrt(v) | Math.sqrt(v) | sqrt(v) | 
| max in array | max(v) | math.max(...v) | max(v) | |
| if in array | 'a' in v | v.indexOf('a') | in_array('a', v) |  | 
| repeat v | v*1 | v.repeat(1) | str_repeat(v, 1) | v.repeat(1) |
| count value in v | v.count('a') | (v.match(new RegExp(a, "g")) || []).length | substr_count(v, 'a') |  |
| count values in arr | arr.count('a') | v.filter(elt => elt === a).length | array_count_values(v) |  |
| first upper in a string | title() | | ucwords(v) | |
| substr string | v[0:len(v)] | v.substring(0, v.length) | substr(v, 0, strlen(v)) |  |
| min alphabet | string.ascii_lowercase | String.fromCharCode(...Array(123).keys()).slice(97) | range('a', 'z') | |
| maj alphabet | string.ascii_uppercase | String.fromCharCode(...Array(91).keys()).slice(65) | range('A', 'Z') | |
| to lower case | v.lower() | v.toLowerCase() | strtolower(v) | |
| to upper case | v.upper() | v.toUpperCase() | strtoupper(v) | |
| init array of n | list(range(0,n+1)) | [...Array(n+1).keys()] | range(0,n) | |
| array sum | sum(arr) | arr.reduce((previousValue, currentValue) => previousValue + currentValue, 0) | array_sum(arr) | |
| int to binary | bin(v)/format(v, "b") | | | |
| remove duplicates | list(set(v)) | [...new Set(v)] | | |