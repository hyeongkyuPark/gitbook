---
description: '조건의 참, 거짓에 따라서 분기하는 조건문 if'
---

# 조건문 if

## 📕 if-else

* 조건문 if\(\) {}는 괄호안에 조건문이 참일경우에만 실행시키는 기능을 가지고 있음
* else {}는 if문의 조건문이 거짓일 경우에 실행되는 블록
* else if\(\) {} 는 if문의 조건문이 거짓일 경우 다시 한번 조건문을 통해 분기시킴

```markup
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta http-equiv="X-UA-Compatible" content="IE=edge">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title></title>
</head>
<body>
  <h1>Conditional statements</h1>
  <h2>Program</h2>
  <script>
    document.write('1<br/>');
    document.write('2<br/>');
    document.write('3<br/>');
    document.write('4<br/>');
  </script>
  <h2>IF-true</h2>
  <script>
    document.write('1<br/>');
    if(true) {
      document.write('2<br/>'); // 조건이 true면 실행
    } else {
      document.write('3<br/>');// 조건이 false면 실행
    }
    document.write('4<br/>');
  </script>
  <h2>IF-false</h2>
  <script>
    document.write('1<br/>');
    if(false) {
      document.write('2<br/>');
    } else {
      document.write('3<br/>');
    }
    document.write('4<br/>');
  </script>
</body>
</html>
```

{% embed url="https://codepen.io/hyeongkyupark/pen/GRWdxJb" %}



