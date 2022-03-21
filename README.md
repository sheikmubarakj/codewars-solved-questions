<div align="center">
  <img height="60" src="https://img.icons8.com/color/344/javascript.png">
  <h1>Codewars Solved Questions</h1>
</div>


###### 1. Complete the solution so that the function will break up camel casing, using a space between words.

```Example
"camelCasing"  =>  "camel Casing"
"identifier"   =>  "identifier"
""             =>  ""
```

<details><summary><b>Answer</b></summary>
<p>

#### Solution: 1

```
function solution(string) {
  return(string.replace(/([A-Z])/g, ' $1'));
}
```
#### Solution: 2

```
function solution(string) {
  string = string.split('').map(function (el) {
    if (el === el.toUpperCase()) {
      el = ' ' + el
    }
    return el
  })
  return string.join('')
}
```

</p>
</details>

