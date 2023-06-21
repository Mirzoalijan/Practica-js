## Practica 
```js
const result = ('b'+'a'+ +'a'+'a').toLowerCase()
console.log(result);
```
## 1
```js
function isEmpty(str) {
    return str === '';
  }
  console.log(isEmpty(""));
```
## 2
```js
function formatName(firstName, lastName) {
    return `${lastName}, ${firstName}`;
  }
  console.log(formatName('John', 'Doe')); 
  console.log(formatName('Jane', 'Smith'));
```
## 3
```js
function isStringLengthEven(str) {
    return str.length % 2 === 0;
  }
console.log(isStringLengthEven("apple"));  
console.log(isStringLengthEven("pears"));
console.log(isStringLengthEven("cherry"));
```
## 4
```js
function isLastCharacterN(text) {
    return text.at(-1).includes("n")

}
console.log(isLastCharacterN("nllln"));
console.log(isLastCharacterN("salom"));
```
## 5
```js
function repeatString(txt) {
    return txt.repeat(2)
}
console.log(repeatString("meet"));
```
## 6
```js
function countCapitalLetters(str) {
    let count = 0;
    for (let i = 0; i < str.length; i++) {
      if (str[i] === str[i].toUpperCase() && str[i] !== str[i].toLowerCase()) {
        count++;
      }
    }
    return count;
  }
console.log(countCapitalLetters("fvLzpxmgXSDrobbgMVrc"));
console.log(countCapitalLetters("mqeytbbjwqemcdrdsyvq"));  
```
## 7
```js
function calculate(num1, num2, operator) {
    switch (operator) {
      case '+':
        return num1 + num2;
      case '-':
        return num1 - num2;
      case '*':
        return num1 * num2;
      case '/':
        return num1 / num2;
      default:
        return NaN;
    }
  }
  console.log(calculate(1, 2, '+'));
  console.log(calculate(1, 2, '-'));
  console.log(calculate(1, 2, '*'));
```
## 8
```js
function res(str) {
    return str.split("-").length
}
console.log(res("sa-lo-m"));
```

## 9
```js
function groupCharacters(txt) {
    let evenChars = '';
    let oddChars = '';
    for (let i = 0; i < txt.length; i++) {
      if (i % 2 == 0) {
        evenChars += txt[i];
      }
      else {
        oddChars += txt[i];
      }
    }
  

    return `${evenChars} ${oddChars}`;
  }
  console.log(groupCharacters("mubashir"));
  console.log(groupCharacters("edabit"));
```
## 10
```js
function res(str) {
    return str.split("potato").length-1
}
console.log(res("potatopotato"));
```
## 11
```js
function countCapitalLetters(str) {
    let count = '';
    for (let i = 0; i < str.length; i++) {
      if (str[i] === str[i].toLowerCase()) {
          count += str[i]
      }
    }
    return count;
  }
console.log(countCapitalLetters("UcUNFYGaFYFYGtNUH"));
```
## 12
```js
function modifyLast(str,last) {
    let num = ''
     num = str.charAt(str.length-1)
    return str + num.repeat(last-1)
}
console.log(modifyLast("Hello",3));
```
## 13
```js
function firstLast(num) {
    return num[0] + num.at(-1)
}
console.log(firstLast("ganesh"));
```
## 14
```js
function toInt(str) {
  return Number(str);
}
console.log(toInt("77"));

function toStr(num) {
  return num.toString();
}
console.log(toStr(55));
```

## 15
```js
function isPlural(num) {
    return num.at(-1) === "s"
}
console.log(isPlural("changes"));
console.log(isPlural("change"));
```

## 16
```js
function reverseCapitalize(str) {
    return str.split('').reverse().join('').toUpperCase()
      
}
console.log(reverseCapitalize("abc"));
console.log(reverseCapitalize("hellothere"));
```

## 17
```js
function swapName(name) {
    const nameArr = name.split(" ");
    const swappedName = nameArr[1] + " " + nameArr[0];    
    return swappedName;
  }
  console.log(swapName("John Smith"));
  function checkPalindrome(str) {
      return str.at(0) === str.at(-1)
  }
  console.log(checkPalindrome("mom"));
 ```
## 18
```js
function countChar(char, str) {
    const count = str.split(char).length - 1;
    return count;
  }
  console.log(countChar("a","banana"));  
``` 
## 19
```js
function moveCapitalLettersToFront(word) {
    let capitalLetters = "";
    let otherLetters = "";
    
    for (let i = 0; i < word.length; i++) {
      if (word[i] >= "A" && word[i] <= "Z") {
        capitalLetters += word[i];
      } else {
        otherLetters += word[i];
      }
    }
    
    return capitalLetters + otherLetters;
  }
  const word = "hApPy";
const movedWord = moveCapitalLettersToFront(word);
console.log(movedWord); 
```
## 20
```js
function reverseAndConcat(i) {
    const reversed = i.toString().split("").reverse().join("");
    const concatenated = reversed + i.toString();
    return concatenated;
  }
  console.log(reverseAndConcat(123456789));
```
## 21
```js
function joinSomething(a) {
    return "something " + a;
  }
  console.log(joinSomething("is better than nothing"));
```
## 22
```js
function stringInt(str) {
    return Namber(str)
}
console.log("6");
```
## 23
```js
function joinSomething(a) {
    return "Hello " + a;
  }
  console.log(joinSomething("Matt"));
```
## 24
```js
function isStringLengthEqual(str1, str2) {
    return str1.length === str2.length;
  }
  console.log(isStringLengthEqual("AB","CD"));
  console.log(isStringLengthEqual("ABC","DE"));
```
## 25
```js
function replaceVowels(str) {
    return str.replace(/[aeiou]/g, function(match) {
      switch(match) {
        case 'a': return '1';
        case 'e': return '2';
        case 'i': return '3';
        case 'o': return '4';
        case 'u': return '5';
      }
    });
  }
console.log(replaceVowels("karachi"));  
console.log(replaceVowels("chembur"));  
console.log(replaceVowels("khandbari"));  
```
## 26
```js
function removeABC(str) {
    if (!/[abc]/.test(str)) {
      return null;
    }
    return str.replace(/[abc]/g, '');
  }
    console.log(removeABC('abcdefg')); 
    console.log(removeABC('xyz')); 
    console.log(removeABC('abcabcabc'));
```"# Practica-js" 
