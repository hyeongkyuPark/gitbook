---
description: 함수 용어와 활용정리
---

# 함수의 활용

## 함수 사용 이유

* 반복적으로 사용되는 코드를 한개의 함수로 정의하여 재사용
* 수정과 유지보수가 용이하게 하기 위해 사



## 매개변수

* 함수를 정의할때 넘어오는 값을 매개변수라고 함
* function sum\(a, b\){} 이 함수에서 매개변수는 a와 b



## 인자

* 함수를 사용할 때 실제로 넘겨주는 매개변수 값을 인자라고 함
* sum\(5, 10\)에서 인자는 5와 10



## 반환값

* 반환값은 함수의 실행 결과로 돌려주는 값
* 반환값은 있을수도 있고 없을수도 있음\(반환값을 입력하지 않으면 기본값 undefined 반환\)
* return 반환값;의 형태로 작성하고, return 뒤에 오는 내용은 전부 무시됨\(return시 함수 종료\)

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
  <h1>함수</h1>
  <h2>
    function add(a, b) { return a+b; }
  </h2>
  <script>
    // 매개변수 a, b를 받아 서로 더한 값을 반환해주는 함수
    function add(a, b) { return a+b; }
  </script>
  <p>add(5, 10) ? </p>
  <script>
//     인자로 5와 10을 전달하여 결과값 출력
    document.write(add(5, 10));
  </script>
</body>
</html>
```

{% embed url="https://codepen.io/hyeongkyupark/pen/MWpXbGa" %}



