### Sass Basics

================

sass를 사용하기 전에 프로젝트에 셋업해야 한다.

### Preprocessing

---

CSS는 무거워지거나 복잡해져 유지하기가 힘들 수 있다.
이것이 프리프로세서가 도울 수 있는 부분이다.
Sass는 CSS에 아직 없는 중첩, 믹스인, 상속, 등등의 특징들로
건실하고 유지보수 가능한 CSS를 만드는데 도움을 줄 것이다.

한번 Sass로 보수하고 나면 Sass파일을 웹사이트에서 사용가능한
일반적인 Css파일로 저장할 수 있게 될 것이다.

이 일은 터미널에서 할 수 있다. Sass가 설치되면,
Sass를 Css로 Sass 명령어를 사용해 컴파일 할 수 있게 될 것이다.
Sass에게 어디서부터 어디까지 css를 빌드해야 할지 말해야 할 것이다.
예를들어 터미널에 Sass input.scss output.css를 입력하면
단일 sass파일인 input.scss파일을 가져와서 output.css파일로 컴파일할 것이다.

또한 개별 파일들 혹은 폴더들을 --watch 플래그 로 지켜볼 수 있다.
watch 플래그로 Sass가 소스파일들의 변화를 지켜보게 하다가 sass를 저장하는 시점에
다시 컴파일하게 하는 것이다.
만약 input.scss파일을 보게하고 싶다면 아래와같이 watch 플래그 명령어를 추가하면 된다.

```
sass --watch input.scss output.css
```

입력과 출력으로 폴더경로를 작성해도 된다. 그럴 떈 colon으로 구분해주면 된다.

```
sass --watch app/sass:public/stylesheets
```

sass는 app/sass폴더 안에있는 모든 파일들의 변화를 지켜보게 될 것이며,
public/styledsheets폴더에 css를 컴파일 할 것이다.
