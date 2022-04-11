## 📝 버킷리스트 구현 과제

---

1. 요구사항<br>
   ✔️ `border` 모양 구현<br>
   ✔️ 리스트 `hover` 하이라이팅<br>
   ✔️ 리스트 `hover` 호박 이미시 변경<br>
   ✔️ 백그라운드 이미지 사용<br>

---

2. 구현 결과물

- 기본 화면
  <img width="1383" alt="스크린샷 2022-04-03 오후 3 57 52" src="https://user-images.githubusercontent.com/97894417/161416055-14ee9f55-cbf7-4c03-87a3-876e15122115.png">

- 리스트에 마우스 `hover` 화면
  <img width="1384" alt="스크린샷 2022-04-03 오후 3 58 09" src="https://user-images.githubusercontent.com/97894417/161416063-06ce49b3-993d-4ed8-86ce-65fecd9bc255.png">

---

3. 새로 알게된 점

- 백그라운드 속성도 단축속성으로 적을 수 있다는 점을 알았다.
- `border-radius`속성 중 네귀퉁이 값을 자유자재로 줄 수 있다. (특이한 모양 가능)

---

4. 어려웠던 점

- 백그라운드 속성 축약표현으로 적던 중 `background-size` 값이 적용이 안되는 문제를 겪었다.
  - 해결볍 : 축약형 구문에 `background-size` 값을 포함하려면 `background-position` 값도 같이 적어줘야했다! 또한 두 값사이는 슬래시(/)로 구분해주어야 한다.
  ```css
  body {
    background-image: url("img.png");
    background-repeat: no-repeat;
    background-position: center;
    background--size: cover;
  }
  ```
  축약형
  ```css
  body {
    background: url("") no-repeat center/cover;
  }
  ```
