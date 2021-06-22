---
description: 반복문에서 많이 사용되는 자료구조인 배열에 대해서 학습
---

# 배열\(Array\)

## 📕 배열

* 배열은 여러개의 값들을 하나로 묶는 리스트
* 배열은 '\['와 '\]' 사이에 값들을 ','로 구분하여 선언 \( \['phg', '12345'\] \)
* \['phg', '12345'\] 에서 첫번째 값은 배열의 0번 인덱스\(index\)의 값이라고 함
* 배열의 값을 가져오는 방법 : "배열\[인덴스 번호\]"
* 배열의 길이를 가져오는 방법 :  "배열.length"
* 배열에 값을 추가하는 방법 : "배열.push\(추가할 값\)"
* 여러가지 명령어들이 있음

{% embed url="https://developer.mozilla.org/ko/docs/Web/JavaScript/Reference/Global\_Objects/Array" %}

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
  <h1>Array</h1>
  <h2>Syntax</h2>
  <script>
    var coworkers = ["egoing", "phg"];
    document.write(coworkers);
  </script>
  <h2>get</h2>
  <script>
    // index 0번 = 배열의 첫번째
    document.write(coworkers[0]); // 배열의 첫번째 값 "egoing"
    document.write('<br />'); // 개행 문자
    document.write(coworkers[1]); // 배열의 두번째 값 "phg"
    
  </script>
  <h2>push</h2>
  <script>
    coworkers.push('pushMember');
    document.write(coworkers);
  </script>
  <h2>length</h2>
  <script>
    document.write(coworkers.length);
  </script>
</body>
</html>
```

{% embed url="https://codepen.io/hyeongkyupark/pen/dyvKMed" %}



