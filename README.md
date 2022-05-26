# Equivalence in languages


|v : variable| Python | JavaScript | PHP | Java |
| --- | --- | --- | --- |--- |
| array to string | "".join(v) | v.join("") | implode("", v) |
| string to array | list(v) | v.split("") | explode("", v)/str_split(v) |
| add in array | arr.append(v) | arr.push(v) | $arr[] = v | |
| reverse string | v[::-1] | v.split("").reverse().join("") | strrev(v) |  |
| reverse array | v[::-1] | v.reverse() | array_reverse(v) |  |
| show v | print(v) | console.log(v) | echo v/print_r(v) |System.out.println(v) |
| sort array | v.sort(key=len, reverse=False) | v.sort() | sort(v)/rsort(v) | |
| numerical value | int(v) | parseInt(v) | intval(v) |  |
| string value | str(v) | v.toString() | strval(v) | |
| sqrt | math.sqrt(v) | Math.sqrt(v) | sqrt(v) | 
| max in array | max(v) | math.max(...v) | max(v) | |
| if in array | 'a' in v | v.indexOf('a') | in_array('a', v) |  | 
| repeat v | v*1 | v.repeat(1) | str_repeat(v, 1) |  |
| count value in v | v.count('a') |  | substr_count(v, 'a') |  |
| count values in arr | arr.count('a') |  | array_count_values(v) |  |
| first upper in a string | title() | | ucwords(v) | |
| substr string | v[0:len(v)] | v.substring(0, v.length) | substr(v, 0, strlen(v)) |  |
| arr 0-n | list(range(0,n+1)) |  | range(0,n) | |
| min alphabet | string.ascii_lowercase | String.fromCharCode(...Array(123).keys()).slice(97) | range('a', 'z') | |
| maj alphabet | string.ascii_uppercase | String.fromCharCode(...Array(91).keys()).slice(65) | range('A', 'Z') | |