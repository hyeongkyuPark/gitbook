# 반복문

## while 반목문

* while\(조건문\) {} 이 기본형태
* 조건문아 참이면 블록안에 기능들을 수행
* 모든 기능을 수행했다면 다시 조건문을 확인하고 참이면 반복, 거짓이면 다음으로 넘어감
* while은 블록안에서 조건문에 관한 변수의 값을 변경하여야 함
* while은 끝이 딱 정해지지 않은 반복문에 주로 사용

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
  <h1>while loop</h1>
  <ul>
    <script>
      var i = 0;
      document.write('<li>1</li>');
      while(i < 3) {
        document.write('<li>2</li>');
        document.write('<li>3</li>');
        i++;
      }
      document.write('<li>4</li>');
    </script>
  </ul>
</body>
</html>
```

{% embed url="https://codepen.io/hyeongkyupark/pen/BaWVzaX" %}



## for 반복문

* for\(반복변수 선언; 조건문; 변수증감;\) {}이 기본형태
* 조건문이 참이라면 블록안에 기능들을 수행
* 모든 기능을 수행했다면 변수증감 후 다시 조건문을 확인하고 참이면 반복, 거짓이면 다음으로 넘어감
* for는 블록내에서 변수의 값을 변경할 필요가 없음
* for은 길이나 반복횟수가 정해져있을때 주로 사용

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
  <h1>while loop</h1>
  <ul>
    <script>
      document.write('<li>1</li>');
      for(var i=0; i<3; i++) {
        document.write('<li>2</li>');
        document.write('<li>3</li>');
      }
      document.write('<li>4</li>');
    </script>
  </ul>
</body>
</html>
```

{% embed url="https://codepen.io/hyeongkyupark/pen/yLMEJgM" %}



