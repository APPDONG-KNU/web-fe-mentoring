### ⏰ 모임 일시

03.30 (화) 19시 00분

### 🚢 참여자

박희연, 배해민, 윤영석

### 📖 학습내용

<aside>
  
🧸 **학습목표** "CSS의 개념 & CSS 선택자 & Cascading 순위"

</aside>
    
- **CSS의 개념**

    <img src="https://user-images.githubusercontent.com/88179771/234756704-4ef84d10-1eca-4430-a433-04dd862d8bba.png" width="480" height="270"/>
    
    <img src="https://user-images.githubusercontent.com/88179771/234756719-69725b64-c21b-4829-a64b-e969b9cf5371.png" width="480" height="270"/>
    
- **CSS 선택자**
    
    <img src="https://user-images.githubusercontent.com/88179771/234756736-b3482e44-bdbb-4498-b98b-fd76112cd0fe.png" width="480" height="270"/>
    
    <img src="https://user-images.githubusercontent.com/88179771/234756755-b693a028-56f6-4e4a-a464-0a2eb7e322a2.png" width="480" height="270"/>
        
    <img src="https://user-images.githubusercontent.com/88179771/234756770-c6a51bf7-2cd6-499d-8635-cd13411495bf.png" width="480" height="270"/>
    
    <img src="https://user-images.githubusercontent.com/88179771/234756782-e5d22cca-ebc7-4221-a492-d16e85de048d.png" width="480" height="270"/>
    
- **Cascading 순위**
    
    <img src="https://user-images.githubusercontent.com/88179771/234756786-c4584fa8-f90b-4c96-b0eb-c09c2a276a5d.png" width="480" height="270"/>
        
- **실습** 💻
    
    **index.html 코드**
    
    ```html
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="UTF-8" />
      <meta http-equiv="X-UA-Compatible" content="IE=edge" />
      <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      <title>20230330 웹멘토링</title>
      <link rel="stylesheet" href="./cascading.css" />
      <style>
        * {
          font-size: 16px;
          font-weight: 400;
          margin: 0;
          padding: 0;
          color: black;
        }
        a {
          text-decoration: none;
          cursor: initial;
        }
        .container {
          background-color: brown;
        }
        .container h2 {
          font-size: 32px;
        }
        #header {
          color: white;
        }
      </style>
    </head>
    <body>
      <div class="container">
        제목 영역
        <h1 id="header">Heading 1</h1>
        <h2>Heading 2</h2>
        <h3>Heading 3</h3>
        <h4>Heading 4</h4>
        <h5>Heading 5</h5>
        <h6>Heading 6</h6>
      </div>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
      <ul>
        순서가 없는 리스트
        <li>1</li>
        <li>2</li>
        <li>3</li>
        <li>4</li>
      </ul>
      <ol>
        <li>1</li>
        <li>2</li>
        <li>3</li>
        <li>4</li>
      </ol>
      <ul>
        내가 좋아하는 음식
        <li>
          과일
          <ul>
            <li>복숭아</li>
            <li>사과</li>
          </ul>
        </li>
        <li>배달음식</li>
      </ul>
      <a href="https://www.google.com">구글 바로가기</a>
    </body>
  </html>
    ```
    
    **결과**
    
    <img src="https://user-images.githubusercontent.com/88179771/234758936-850022cf-9c28-4511-9596-4ab4a7ebe4ba.png" width="100%" />
    
    **cascading.html 코드**
    
    ```html
  <!DOCTYPE html>
  <html lang="en">
    <head>
      <meta charset="UTF-8" />
      <meta http-equiv="X-UA-Compatible" content="IE=edge" />
      <meta name="viewport" content="width=device-width, initial-scale=1.0" />
      <title>Cascading</title>
      <link rel="stylesheet" href="./cascading.css" />
    </head>
    <body>
      <div class="container">
        <div id="box" class="inner">
          <p class="txt1 text">
            Lorem, ipsum dolor sit amet consectetur adipisicing elit. Voluptates
            tempore hic dolores odit distinctio repellat beatae eius explicabo
            doloribus quidem labore sit, eaque et voluptatem sint ad maiores at!
            Consequuntur?
          </p>
          <p class="txt2 text">
            Lorem ipsum dolor sit amet consectetur adipisicing elit. Quo
            assumenda, reiciendis nostrum cum odio fugit perspiciatis nam quia
            eveniet officia maxime eos unde quaerat quae doloribus explicabo
            dolores recusandae quis.
          </p>
          <p class="txt3 text">
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Soluta
            voluptas, animi temporibus aut possimus sint et, aliquam, magni
            eligendi optio eveniet quis sapiente voluptatibus blanditiis pariatur
            neque doloribus modi autem.
          </p>
        </div>
      </div>
    </body>
  </html>
    ```
    
    **cascading.css 코드**
    
    ```html
  * {
  font-size: 20px;
  font-size: 32px;
  }

  .txt1 {
    font-size: 72px;
  }

  #box {
    background-color: chartreuse;
  }

  .text {
    background-color: yellow;
  }

  .inner {
    background-color: red !important;
  }
    ```
    
    **결과**
    
    <img src="https://user-images.githubusercontent.com/88179771/234759549-9dd8a9d5-d730-4cfb-8753-b6d4552e9539.png" width="100%" />

### ✔️ 체크리스트

- [x]  인증샷 남기기
