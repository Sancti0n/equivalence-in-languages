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
JavaScript : v.sort()
PHP : sort(v)/rsort(v)
Java : 
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
    List<String> L = Arrays.asList(v);
    if (L.contains("a")) {return true}
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
Java : 
```

## String to upper case
```python
Python : v.upper()
JavaScript : v.toUpperCase()
PHP : strtoupper(v)
Java : 
```

## Substring
```python
Python : v[0:len(v)]
JavaScript : v.substring(0, v.length)
PHP : substr(v, 0, strlen(v))
Java : 
```

## First upper in a string
```python
Python : title()
JavaScript :
PHP : ucwords(v)
Java : 
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