# Equivalence in languages

- [Type of v ](https://github.com/Sancti0n/equivalence-in-languages#type-of-v)
- [Array -> string](https://github.com/Sancti0n/equivalence-in-languages#array---string)
- [String -> array](https://github.com/Sancti0n/equivalence-in-languages#string---array)
- Alphabet Array
    - [Array of lower case letters](https://github.com/Sancti0n/equivalence-in-languages#array-of-lower-case-letters)
    - [Array of upper case letters](https://github.com/Sancti0n/equivalence-in-languages#array-of-upper-case-letters)
- [Repeat a string](https://github.com/Sancti0n/equivalence-in-languages#repeat-a-string)
- [Add elt in array](https://github.com/Sancti0n/equivalence-in-languages#add-elt-in-array)
- Reverse
    - [Reverse a string](https://github.com/Sancti0n/equivalence-in-languages#reverse-a-string)
    - [Reverse an array](https://github.com/Sancti0n/equivalence-in-languages#reverse-an-array)
- [Show v](https://github.com/Sancti0n/equivalence-in-languages#show-v)
- [Numerical value](https://github.com/Sancti0n/equivalence-in-languages#numerical-value)
- [String value](https://github.com/Sancti0n/equivalence-in-languages#string-value)
- [Sort array](https://github.com/Sancti0n/equivalence-in-languages#sort-array)
- [SQRT](https://github.com/Sancti0n/equivalence-in-languages#sqrt)
- [Maximum in array](https://github.com/Sancti0n/equivalence-in-languages#maximum-in-array)
- [If elt in array](https://github.com/Sancti0n/equivalence-in-languages#if-elt-in-array)
- [Sum of one array](https://github.com/Sancti0n/equivalence-in-languages#sum-of-one-array)
- [Init array of n number](https://github.com/Sancti0n/equivalence-in-languages#init-array-of-n-number)
- Lower & upper case
    - [String to lower case](https://github.com/Sancti0n/equivalence-in-languages#string-to-lower-case)
    - [String to upper case](https://github.com/Sancti0n/equivalence-in-languages#string-to-upper-case)
- [Substring](https://github.com/Sancti0n/equivalence-in-languages#substring)
- [First upper in a string](https://github.com/Sancti0n/equivalence-in-languages#first-upper-in-a-string)
- [Int -> binary](https://github.com/Sancti0n/equivalence-in-languages#int---binary)
- [Replace value in string](https://github.com/Sancti0n/equivalence-in-languages#replace-value-in-string)
- Count
    - [Count value in string](https://github.com/Sancti0n/equivalence-in-languages#count-value-in-string)
    - [Count value in array](https://github.com/Sancti0n/equivalence-in-languages#count-value-in-array)
- [Remove duplicates](https://github.com/Sancti0n/equivalence-in-languages#remove-duplicates)
- [Array of strings in array of floats](https://github.com/Sancti0n/equivalence-in-languages#array-of-strings-in-array-of-floats)
- [Clone array](https://github.com/Sancti0n/equivalence-in-languages#clone-array)
- [Concat array](https://github.com/Sancti0n/equivalence-in-languages#concat-arrays)
- [Int to int array](https://github.com/Sancti0n/equivalence-in-languages#int-to-int-array)
- [Multiply all values in array](https://github.com/Sancti0n/equivalence-in-languages#multiply-all-values-in-array)

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
    String w = "";
    for (char c = 'a'; c <= 'z'; c++) w += c;
    String[] arr = w.split("");

Output -> ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']
```

## Array of upper case letters
```python
Python : list(string.ascii_uppercase)
JavaScript : String.fromCharCode(...Array(91).keys()).slice(65).split("")
PHP : range('A', 'Z')
Java :
    String w = "";
    for (char c = 'A'; c <= 'Z'; c++) w += c;
    String[] arr = w.split("");

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
    int [] myArr = {1,3,5,7,9}
    int[] r = new int[myArr.length];
    for(int i=0;i<myArr.length; i++) {
      r[i] = myArr[myArr.length-i-1];
    }

    Collections.reverse(Arrays.asList(v))
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
Java :
    Integer.parseInt(v)
    Double.parseDouble(v)
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
JavaScript : Math.max(...v)
PHP : max(v)
Java :
    int max = v[0];
    for (int i=1;i<v.length;i++) {
        max = Math.max(max, v[i]);
    }
```

## If elt in array
```python
Python : 'a' in v
JavaScript : v.indexOf('a')
PHP : in_array('a', v) / str_contains(v, 'a')
Java :
    import java.util.Arrays
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
JavaScript : [...Array(n+1).keys()] / Array.from(Array(n)).map((e,i)=>i+1)
PHP : range(0,n)
Java :
    import java.util.Arrays;
    int[] arr = new int[n];
    Arrays.setAll(arr, i->i+1); / for reversed array : Arrays.setAll(arr, i->n-i);
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

Python : v.title()
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
JavaScript : v.toString(2)
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
Java :
    # for one character
    String.join("", v).length() - String.join("", v).replace("a", "").length()

    int count = 0;
    for (int i=0;i<v.length;i++) if (v[i] == "a") count++;

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

## Clone array
```python
Python : arr = array.copy()
JavaScript : let arr = [...array]
PHP : a = v
Java :
    import java.util.Arrays
    String[] array = {"a", "b", "c"}
    String[] copiedArray = Arrays.copyOfRange(array, 0, array.length)
```

## Concat arrays
```python
Input -> arr1 = [1,2,3], arr2 = [4,5,6]

Python : arr1 + arr2
JavaScript : arr1.concat(arr2)
PHP : array_merge($arr1, $arr2);
Java :
    import java.util.Arrays;
    int[] array1 = {1, 2, 3};
    int[] array2 = {4, 5, 6};

    int aLen = array1.length;
    int bLen = array2.length;
    int[] result = new int[aLen + bLen];

    System.arraycopy(array1, 0, result, 0, aLen);
    System.arraycopy(array2, 0, result, aLen, bLen);

Output -> [1,2,3,4,5,6]
```

## Int to int array
```python
Input -> v = 156

Python : list(map(int, str(v)))
JavaScript : Array.from(String(v), Number);
PHP : array_map('intval', str_split($v));
Java :
    import java.util.ArrayList;
    ArrayList<Integer> array = new ArrayList<Integer>();
    do {
        array.add(0, temp % 10);
        temp /= 10;
    } while (v > 0);

Ouput -> [1,5,6]
```

## Multiply all values in array
```python
Input -> v = [1,2,3]

Python :
    import math
    math.prod(v)
JavaScript : v.reduce((a, b)=> a*b, 1)
PHP : array_product($v);
Java:
    int m = 1;
    for(int i=0;i<v.length;i++) {
        m *= v[i];
    }

Output -> 6
```

## Code Golf
```python
JavaScript:
    Addition : madAdd=(a,b)=>a- -b
    Soustraction : madSub=(a,b)=>a+~b+1
    Multiplication : madMul=(a,b)=>~~(a/(1/b)+.5)
    Division : madDiv=(a,b)=>a*b**-1
    Modulus : madMod=(a,b)=>!b?NaN:a-b*~~(a/b)
    Power : madPow=(a,b)=>!b?1:madPow(a,b-1)/(1/a)
    Infinity : f=x=>1/0
```