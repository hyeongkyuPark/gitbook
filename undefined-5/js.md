---
description: html파일과 js파일을 분리
---

# JS파일로 나누기

## 목적

* 코드의 가독성을 위해 html과 js파일을 분리
* 여러 html파일에서 같은 javascript 코드가 쓰일때 더 편리하게 사용가능
* 수정시 여러곳에서 사용하고 있더라도 js파일 하나만 수정하면 전부 수정됨
* 결국 코드 재사용성과 코드 가독성을 위함

```markup
<!-- index.html -->
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
  <!-- 분리한 스크립트 파일 불러오 -->
  <script src="./colors.js">
</body>
</html>
```

```javascript
    // colors.js
    var body = {
      target: document.querySelector('body'),
      setBackgroundColor: function(color) {
        this.target.style.backgroundColor = color;
      },
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
```

