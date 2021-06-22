# 객체\(Object\)

## 객체

* 여러개의 연관있는 함수와 여러개의 연관 있는 변수를 하나로 묶어주는 기능
* 복잡도를 줄이고, 코드 관리를 용이하게 하기위함



## 객체 생성과 읽기 쓰

* "var 객체명 = {속성이름:  속성값,  속성이름:  속성값, } \(= 오브젝트 리터럴\)" 로 객체 생성
* "객체명.속성이름"으로 객체 값 가져오기\(읽기\)
* "객체명.속성이름 = 속성값"으로 객체 값 수정 또는 새로운 속성값 생성\(쓰기\)

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
  <h1>객체(Object)</h1>
  <h2>객체 생성</h2>
  <p>
    var product = {
      name: 'banana',
      price: 1000,
    }
  </p>
  <script>
    // 객체 생성
    var product = {
      name: 'banana', // name 속성 정의
      price: 1000, // price 속성 정의
    }
  </script>
  <h2>객체 값 가져오기</h2>
  <script>
    document.write('product.name: ' + product.name);
    document.write('<br />'); // 개행 문자
    document.write('product.price: ' + product.price);
  </script>
  <h2>객체 값 쓰기</h2>
  <script>
    document.write('쓰기전 product.sale : ' + product.sale); // 값이 없으므로undifined
    product.sale = 200;
    document.write('쓰기후 product.sale : ' + product.sale);
  </script>
</body>
</html>
```

{% embed url="https://codepen.io/hyeongkyupark/pen/wvJXgaw" %}





## 반복문\(for in\)

* 반복문을 사용해 객체의 key값을 전부 순회하며 가져올 수 있음
* "for\(var i in 객체명\){}"으로 사용

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
  <h1>객체(Object)</h1>
  <h2>객체 생성</h2>
  <p>
    var product = {
      name: 'banana',
      price: 1000,
      sale: 500
    }
  </p>
  <script>
    // 객체 생성
    var product = {
      name: 'banana', // name 속성 정의
      price: 1000, // price 속성 정의
      sale: 500,
    }
  </script>
  <h2>Iterate</h2>
  <script>
    // in : 객체에서는 key값을 반복하고, 배열에서는 index값을 반복하여 앞에 선언한 변수에 할당함
    for(var key in product) {
      document.write(key + ' : ' + product[key] + '<br>');
    }
  </script>
</body>
</html>
```

{% embed url="https://codepen.io/hyeongkyupark/pen/jOBKyYy" %}



