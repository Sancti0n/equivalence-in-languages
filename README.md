# Equivalence in languages

[Type of v ](https://github.com/Sancti0n/equivalence-in-languages#type-of-v)

[Array -> string](https://github.com/Sancti0n/equivalence-in-languages#array---string)

[String -> array](https://github.com/Sancti0n/equivalence-in-languages#string---array)

[Array of lower case letters](https://github.com/Sancti0n/equivalence-in-languages#array-of-lower-case-letters)

[Repeat a string](https://github.com/Sancti0n/equivalence-in-languages#repeat-a-string)

[Add elt in array](https://github.com/Sancti0n/equivalence-in-languages#add-elt-in-array)

[Reverse a string](https://github.com/Sancti0n/equivalence-in-languages#reverse-a-string)

[Reverse an array](https://github.com/Sancti0n/equivalence-in-languages#reverse-an-array)

[Show v](https://github.com/Sancti0n/equivalence-in-languages#show-v)

[Numerical value](https://github.com/Sancti0n/equivalence-in-languages#numerical-value)

[String value](https://github.com/Sancti0n/equivalence-in-languages#string-value)

[Sort array](https://github.com/Sancti0n/equivalence-in-languages#sort-array)

[SQRT](https://github.com/Sancti0n/equivalence-in-languages#sqrt)

[Maximum in array](https://github.com/Sancti0n/equivalence-in-languages#maximum-in-array)

[If elt in array](https://github.com/Sancti0n/equivalence-in-languages#if-elt-in-array)

[Sum of one array](https://github.com/Sancti0n/equivalence-in-languages#sum-of-one-array)

[Init array of n number](https://github.com/Sancti0n/equivalence-in-languages#init-array-of-n-number)

[String to lower case](https://github.com/Sancti0n/equivalence-in-languages#string-to-lower-case)

[String to upper case](https://github.com/Sancti0n/equivalence-in-languages#string-to-upper-case)

[Substring](https://github.com/Sancti0n/equivalence-in-languages#substring)

[First upper in a string](https://github.com/Sancti0n/equivalence-in-languages#first-upper-in-a-string)

[Int -> binary](https://github.com/Sancti0n/equivalence-in-languages#int---binary)

[Replace value in string](https://github.com/Sancti0n/equivalence-in-languages#replace-value-in-string)

[Count value in string](https://github.com/Sancti0n/equivalence-in-languages#count-value-in-string)

[Count value in array](https://github.com/Sancti0n/equivalence-in-languages#count-value-in-array)

[Remove duplicates](https://github.com/Sancti0n/equivalence-in-languages#remove-duplicates)

[Array of strings in array of floats](https://github.com/Sancti0n/equivalence-in-languages#array-of-strings-in-array-of-floats)
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
Java : 
    System.out.println(v)
    
    import java.util.Arrays;
    System.out.println(Arrays.toString(v));
```

## Numerical value
```python
Python : int(v)
JavaScript : parseInt(v)
PHP : intval(v)
Java : Integer.parseInt(v)
```

## String value
```python
Python : str(v)
JavaScript : v.toString()
PHP : strval(v)
Java : String.valueOf(v)
```

## Sort array
```python
Python : v.sort(key=len, reverse=False)
JavaScript : v.sort() / if int array v.sort((a,b)=>a-b)
PHP : sort(v)/rsort(v)
Java : 
    import java.util.Arrays
    Arrays.sort(v)
```

## SQRT
```python
Python : math.sqrt(v)
JavaScript : Math.sqrt(v)
PHP : sqrt(v)
Java : 
```

## Maximum in array
```python
Python : max(v)
JavaScript : math.max(...v)
PHP : max(v)
Java : 
```

## If elt in array
```python
Python : 'a' in v
JavaScript : v.indexOf('a')
PHP : in_array('a', v) / str_contains(v, 'a')
Java :
    import java.util.*
    return Arrays.asList(v).contains("a")
```

## Sum of one array
```python
Python : sum(arr)
JavaScript : arr.reduce((previousValue, currentValue) => previousValue + currentValue, 0)
PHP : array_sum(arr)
Java : 
    int sum = 0;
    for (int i=0;i<arr.length;i++) sum = sum + arr[i];
```

## Init array of n number
```python
Python : list(range(0,n+1))
JavaScript : [...Array(n+1).keys()] / new Array(Math.max(...numbers)+ 1 - Math.min(...numbers)).fill().map((d, i) => i + Math.min(...numbers));
PHP : range(0,n)
Java : 
```

## String to lower case
```python
Python : v.lower()
JavaScript : v.toLowerCase()
PHP : strtolower(v)
Java : v.toLowerCase()
```

## String to upper case
```python
Python : v.upper()
JavaScript : v.toUpperCase()
PHP : strtoupper(v)
Java : v.toUpperCase()
```

## Substring
```python
Python : v[0:len(v)]
JavaScript : v.substring(0, v.length)
PHP : substr(v, 0, strlen(v))
Java : v.substring(0,v.length())
```

## First upper in a string
```python
Input -> v = "string"

Python : title()
JavaScript : 
    let arr = v.split(" ")
    for (let i=0;i<arr.length;i++) arr[i] = arr[i][0].toUpperCase() + arr[i].slice(1)
    v = arr.join(" ")
PHP : ucwords(v)
Java :

Output -> "String"
```

## Int -> binary
```python
Python : bin(v)/format(v, "b")
JavaScript :
PHP :
Java : 
```

## Replace value in string
```python
Input -> v = "abracadabra"

Python : v.replace("a", "i") 
JavaScript : v.replace(/a/g, 'i') 
PHP : str_replace("a", "i", v)
Java : v.replace('a', 'i')

Output -> "ibricidibri"
```

## Count value in string
```python
Input -> v = "abracadabra"

Python : v.count("a")
JavaScript : (v.match(new RegExp("a", "g")) || []).length
PHP : substr_count(v, 'a')
Java : v.length() - v.replace("a", "").length()

Output -> 5
```

## Count value in array
```python
Input -> v = ["a","b","r","a","c","a","d","a","b","r","a"]

Python : v.count("a")
JavaScript : v.filter(elt => elt === a).length
PHP : array_count_values(v)["a"]
Java : String.join("", v).length() - String.join("", v).replace("a", "").length()

Output -> 5
```

## Remove duplicates
```python
Input -> v = ["a","b","r","a","c","a","d","a","b","r","a"]

Python : list(set(v))
JavaScript : [...new Set(v)]
PHP : array_unique(v)
Java : 

Output -> ['a', 'r', 'c', 'd', 'b']
```

## Array of strings in array of floats
```python
Input -> v = ["1", "2", "3"]

Python : list(map(float, v))
JavaScript : v.map(Number)
PHP : array_map('floatval', v)
Java :

Output -> [1, 2, 3]
```