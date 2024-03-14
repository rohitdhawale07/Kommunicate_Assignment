### Hosted Link of Project:- https://rohitdhawale07.github.io/Kommunicate_Assignment/
## Javascript code for extracting the value of a specified parameter from a given URL.
``` 
function getUrlParameterValue(url, parameter) {
  var urlWithoutHash = url.split("#")[0];
  var urlParts = urlWithoutHash.split("?");
  if (urlParts.length <= 1) {
    return null;
  }
  var paramsString = urlParts[1];
  var params = paramsString.split("&");
  for (var i = 0; i < params.length; i++) {
    var keyValue = params[i].split("=");
    if (keyValue[0] === parameter) {
      return keyValue[1];
    }
  }
  return null;
}
var url = "https://www.kommunicate.io/poweredby?utm_source=https://www.kommunicate.io/&utm_medium=webplugin&utm_campaign=poweredby";
console.log(getUrlParameterValue(url, "utm_medium")); 
console.log(getUrlParameterValue(url, "utm_campaign"));
```

##  Javascript function for printing a revese number
There is two ways for reversing a number, first way will be using while loop.
```
function reverseNumber(num) {
  var reversed = 0;
  num = Math.abs(num);
  while (num > 0) {
    var digit = num % 10;
    reversed = reversed * 10 + digit;
    num = Math.floor(num / 10);
  }
  return reversed;
}
console.log(reverseNumber(1234));
```
Second way will be using inbuilt methods.
```
function reverseNumber(num) {
  var reversedString = num.toString().split("").reverse().join("");
  var reversedNumber = parseInt(reversedString);
  return reversedNumber;
}

console.log(reverseNumber(1234));
console.log(reverseNumber(987654321));

```

## Describing Best Project
## Quiz Game App inspired by KBC
#### Hosted Link:- https://quiz-kbc-git-main-rohit-dhawales-projects.vercel.app/
[Hosted Link Here](https://quiz-kbc-git-main-rohit-dhawales-projects.vercel.app/)

This is a simple quiz game app built using React. 
The game presents a series of multiple-choice questions to the user and tracks their progress as they answer each question. 
The user can earn money based on the difficulty of the questions.

### Features

- User-friendly interface.
- Multiple-choice questions with varying difficulty levels.
- Timer for each question.
- Dynamic money pyramid reflecting the user's progress.
- Earned money displayed at the end of the game.

 ### Usage
- Launch the app.
- Enter your username to begin the quiz.
- Answer each question within the given time.
- Earn virtual money based on correct answers.
- The game ends when all questions are answered or the timer runs out.
