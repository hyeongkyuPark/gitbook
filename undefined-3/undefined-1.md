---
description: 반복문에서 배열을 사용하는 방법
---

# 배열 반복문

## 반복문에서의 배 활용

* 배열 안에 값이 무수히 많다고 가정할때 배열을 이용해서 웹 사이트에 배열의 순서대로 하나씩 가공하여 보여주려 한다면 코드가 엄청 길어지고 복잡해짐
* 이때 반복문을 이용한다면 데이터의 값이 바뀌거나 데이터가 추가되어도 스크립트 로직은 고치지 않아도 자동으로 데이터에 따라서 변경되게 할 수 있음\(조건문으로 배열의 길이를 사용\)

```markup
<!DOCTYPE html>
<html lang="ko">

<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title></title>
</head>

<body>
  <h1>Loop & Array</h1>
  <script>
    // 배열의 수를 늘려도 자동으로 코드에 반영됨
    var fruits = ['apple', 'orange', 'banana', 'mango'];
  </script>
  <h2>Fruits</h2>
  <ul>
    <script>
      var i = 0;
      
      // 배열의 길이만큼 반복하여 배열의 값들을 가공할 수 있음
      while(i < fruits.length) {
        document.write('<li>'+ fruits[i] +'</li>');
        i++;
      }
    </script>
  </ul>
</body>

</html>
```

{% embed url="https://codepen.io/hyeongkyupark/pen/ExWRgyM" %}



