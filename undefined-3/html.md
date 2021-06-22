---
description: 배열과 반복문을 활용하여 html에 적용
---

# html 적용하기

## html 리스트 색상 변경하기

1. a링크의 element들을 querySelectorAll을 이용해 유사배열에 담음
2. 유사배열의 길이 만큼 반복하여 각 요소들의 스타일 값 변경

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
  <h1><a href="#">홈으로</a></h1>
  <input type="button" value="불 끄기" onclick = "
    var bodyElem = document.querySelector('body');
    // 1. html내의 모든 a태그를 변수 alist에 담음
    var alist = document.querySelectorAll('a');
    if(this.value === '불 끄기') {
      bodyElem.style.backgroundColor = 'black';
      bodyElem.style.color = 'white';
      this.value = '불 켜기';
      // for을 사용해 배열 길이만큼 반
      for(var i = 0; i < alist.length; i++) {
        // 각 요소의 색상을 변
        alist[i].style.color = 'powderblue';
      } 
    } else {
      bodyElem.style.backgroundColor = 'white';
      bodyElem.style.color = 'black';
      this.value = '불 끄기';
      var i = 0;
      // while 반복문을 이용해서 배열의 길이만큼 반
      while(i < alist.length) {
        alist[i].style.color = 'blue';
        i++;
      }
    }          
  " />
  <ul>
    <li><a href="#">1. 기획</a></li>
    <li><a href="#">2. 디자인</a></li>
    <li><a href="#">3. 퍼블리싱</a></li>
    <li><a href="#">4. 프론트</a></li>
    <li><a href="#">5. 백</a></li>
  </ul>
  <p>
    웹사이트를 구축은 크게 기획, 디자인, 퍼블리싱, 개발이라는 4단계를 거쳐서 진행되고 있으며 전체 프로젝트를 총괄하는 PM(Project Manager)와 각 단계의 PL(Project Leader)의 원활한 커뮤니케이션을 통해 성공적인 프로젝트를 완료하는데 목적을 둔다. 여기서 웹디자인 과정은 웹사이트의 컨셉(Concept)에 맞게 구체적인 시각화와 사용성을 높이는데 중요한 역할을 하고 있으며 보다 전문적인 아트디렉터가 투입되기도 한다.
  </p>
</body>
</html>
```

{% embed url="https://codepen.io/hyeongkyupark/pen/bGqKwKv" %}



