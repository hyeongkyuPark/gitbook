# 함수\(Function\)

* function 함수명\(매개변수\) {}이 선언의 기본형태
* 매개변수: 전달할 값\(인자\)
* 사용할 때는 "변수명\(매개변수\)"로 사용

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
  <h1>Function</h1>
  <h2>Basic</h2>
  <ul>
    <script>
      // two 함수 선언
      function two() {
        document.write('<li>2-1</li>');
        document.write('<li>2-2</li>');
      }
      
      document.write('<li>1</li>');
      document.write('<li>2</li>');
      //two 함수 사용
      two();
      document.write('<li>3</li>');
      two();
    </script>
  </ul>
</body>
</html>
```

{% embed url="https://codepen.io/hyeongkyupark/pen/XWMYNpX" %}



