---
description: 객체의 용어와 활용방법
---

# 객체의 활용

## Property

* 클래스안에서 만드는 변수로 함수도 클래스에 포함
* key와 value로 이루어짐
* {key: value, } 형태



## Method

* 클래스 또는 함수 안에서 만드는 함수
* property와 마찬가지로 key와 value로 이루어지는데 value가 function임
* {key: function\(\) {}, }



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
  <input type="button" value="불 끄기" onclick = "lightToggleHandler(this)" />
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
  <script>
    var body = {
      target: document.querySelector('body'), // Property
      setBackgroundColor: function(color) {
        this.target.style.backgroundColor = color;
      }, // Method
      setColor: function(color) {
        this.target.style.color = color;
      },
    } // body 관련 변수와 함수를 묶어서 객체로 만듬
    
    var alist = {
      target: document.querySelectorAll('a'),
      setColor: function(color) {
        for(var i = 0; i < this.target.length; i++) {
          this.target[i].style.color = color;
        }
      },
    } // alist 관련 변수와 함수를 묶어서 객체로 만듬
    
    function lightToggleHandler(self) {
      if(self.value === '불 끄기') {
        body.setBackgroundColor('black');
        body.setColor('white');
        alist.setColor('powderblue');
        self.value = '불 켜기';
      } else {
        body.setBackgroundColor('white');
        body.setColor('black');
        alist.setColor('blue');
        self.value = '불 끄기';
      }
    }    
  </script>
</body>
</html>
```

{% embed url="https://codepen.io/hyeongkyupark/pen/NWpzded" %}



