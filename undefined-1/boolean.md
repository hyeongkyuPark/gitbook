---
description: 비교연산자와 boolean 데이터 타입
---

# 비교연산자와 boolean 데이터 타입

## 📕 비교 연산자

* 동등 연산자\(===\) : 왼쪽 값과 오른쪽 값이 같고, 데이터 타입까지 일치해야 참\(true\)을 반환
* 일치 연산자\(==\) : 왼쪽 값과 오른쪽 값만을 비교하여 같으면 참\(true\)을 반환
* &lt;, &gt; : 값을 비교하는 연산자로 크거나 작음을 판단하여 참\(true\), 거짓\(false\) 반환
* &lt;=, &gt;= : 값을 비교하는 연산자로 크거나같음, 작거나 같음을 판단하여 참\(true\), 거짓\(false\) 반환

{% embed url="https://tcpschool.com/javascript/js\_operator\_comparison" %}

* 여기서 반환하는 값 ture, false의 데이터 타입을 Bollean 이라함

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
  <h1>Comparison operators & Boolean</h1>
  <h2>===(동등 연산자) : 값과 데이터타입이 모두 같아야 참</h2>
  <h3>1===1</h3>
  <script>
    document.write(1===1); // 참
  </script>
  <h3>1===2</h3>
  <script>
    document.write(1===2); // 거짓
  </script>
  <h3>1==='1'</h3>
  <script>
    document.write(1===1); // 거짓
  </script>
  <h3>1=='1'</h3>
  <script>
    document.write(1===2); // 참
  </script>
  <h3>1&lt;2</h3>
  <script>
    document.write(1<2); // 참
  </script>
  <h3>1&lt;1</h3>
  <script>
    document.write(1<1); // 거짓
  </script>
  <h3>1&lt;=1</h3>
  <script>
    document.write(1<=1); // 참
  </script>
  <h2>true, false : Boolean 타입</h2>
</body>
</html>
```

{% embed url="https://codepen.io/hyeongkyupark/pen/MWpGQRJ" %}



