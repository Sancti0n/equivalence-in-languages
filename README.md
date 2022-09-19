# Equivalence in languages

## Type of v 
```python
Python : type(v)
JavaScript : typeof v
PHP : gettype(v)
Java : v.getClass().getSimpleName()
```

## Array -> string 
```python
Input -> v = ["S", "t", "r", "i", "n", "g"]

Python : "".join(v)
JavaScript : v.join("")
PHP : implode("", v)
Java : String.join("", v)

Output -> "String"
```

## String -> array 
```python
Input -> v = "String"

Python : list(v)
JavaScript : v.split("")
PHP : str_split(v) / explode(" ", v) if separator != ""
Java : v.split("")

Output -> ["S", "t", "r", "i", "n", "g"]
```

## Array of lower case letters
```python
Python : list(string.ascii_lowercase)
JavaScript : String.fromCharCode(...Array(123).keys()).slice(97).split("")
PHP : range('a', 'z')
Java : 

Output -> ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']
```

## Array of upper case letters
```python
Python : list(string.ascii_uppercase)
JavaScript : String.fromCharCode(...Array(91).keys()).slice(65).split("")
PHP : range('A', 'Z')
Java : 

Output -> ['A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z']
```

## Repeat a string
```python
Input -> v = "String", a = 3

Python : v*a
JavaScript : v.repeat(a)
PHP : str_repeat(v, a)
Java : v.repeat(a)

Output -> "StringStringString"
```

## Add elt in array
```python
Input -> arr = [], v = "S"

Python : arr.append(v)
JavaScript : arr.push(v)
PHP : arr[] = v
Java :
    int arr[] = {1,2,3,4,5,6};
    int n = arr.length;
    int newArr[] = new int[n+1];
    int value = 7;
    for(int i = 0; i<n; i++) { newArr[i] = arr[i]; }
    newArr[n] = value;
    
    Integer arr[] = {1,2,3,4,5,6};
    ArrayList<Integer> arrayList = new ArrayList<Integer>(Arrays.asList(arr));
    arrayList.add(7);
    arr = arrayList.toArray(arr);  

Output -> ["S"]
```

## Reverse a string
```python
Input -> v = "String"

Python : v[::-1]
JavaScript : v.split("").reverse().join("")
PHP : strrev(v)
Java :
    char ch[]=v.toCharArray();  
    String rev="";  
    for(int i=ch.length-1;i>=0;i--) { rev+=ch[i]; }

Output -> "StringStringString"
```

## Reverse an array
```python
Input -> v = ["S", "t", "r", "i", "n", "g"]

Python : v[::-1]
JavaScript : v.reverse()
PHP : array_reverse(v)
Java :
    String [] myArray = {1,3,5,7,9};
    Collections.reverse(Arrays.asList(myArray));
    Arrays.asList(myArray);

Output -> ["g", "n", "i", "r", "t", "S"]
```

## Show v
```python
Python : print(v)
JavaScript : console.log(v)
PHP : echo v / print_r(v) if v is an array
Java : System.out.println(v)
```


|v : variable| Python | JavaScript | PHP | Java |
| --- | --- | --- | --- |--- |
| sort array | v.sort(key=len, reverse=False) | v.sort() | sort(v)/rsort(v) | |
| numerical value | int(v) | parseInt(v) | intval(v) | Integer.parseInt(v) |
| string value | str(v) | v.toString() | strval(v) | String.valueOf(v) |
| replace value in str | | | | v.replace('a) |
| sqrt | math.sqrt(v) | Math.sqrt(v) | sqrt(v) | 
| max in array | max(v) | math.max(...v) | max(v) | |
| if in array | 'a' in v | v.indexOf('a') | in_array('a', v) |  | 
| count value in v | v.count('a') | (v.match(new RegExp(a, "g")) || []).length | substr_count(v, 'a') |  |
| count values in arr | arr.count('a') | v.filter(elt => elt === a).length | array_count_values(v) |  |
| first upper in a string | title() | | ucwords(v) | |
| substr string | v[0:len(v)] | v.substring(0, v.length) | substr(v, 0, strlen(v)) |  |
| to lower case | v.lower() | v.toLowerCase() | strtolower(v) | |
| to upper case | v.upper() | v.toUpperCase() | strtoupper(v) | |
| init array of n | list(range(0,n+1)) | [...Array(n+1).keys()] | range(0,n) | |
| array sum | sum(arr) | arr.reduce((previousValue, currentValue) => previousValue + currentValue, 0) | array_sum(arr) | |
| int to binary | bin(v)/format(v, "b") | | | |
| remove duplicates | list(set(v)) | [...new Set(v)] | | |