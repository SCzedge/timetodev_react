개발은처음이라 엠소프트
초심자용 내용 다음시간에는 useState 특화쪽인듯. 추후 후속 이메일준다함.




리액트 소개 및 개발환경 구축

1. jsx이해와 문법
2. component이해 및 유형
3. 컴포넌트입력 props
4. 컴포넌트 출력state이해
5. 리액트 이벤트 & dom제어 ref
6. 컴포넌트 라이프사이클 관리


## nvm

### install
https://github.com/coreybutler/nvm-windows/releases

### command
버젼확인 : ``nvm version``  
설치된 nvm목록 확인 : ``nvm ls``  
버전 변경 : ``nvm use version``  



## yarn
 npm보다 개선됨.

### install
npm install -g yarn

### command
버젼확인 : ``yarn -v``  
yarn 프로젝트 생성 : ``yarn init``  


## VSC_extension
- reactjs code snippets

## cra node_modules 복원
프로젝트 안에서``yarn``입력.  

## JSX
- js에 xml 문법을 추가한 js확장문법  
- js코드와html 코드를 동일 컴포넌트에서 제어가능  
- 리액트에서 실제적으로 화면을 표현해주는 html비슷한
return 구문 안에있는 코드들. xml 표시법으로 표시하는 html 빌드시 js로 변환됨.

## JSX 규칙
- 닫는태그 반드시.
- 최상위 태그는 하나 이거나 fragment요소로 감싸주어야.
- jsx내 js코드는 {}블록안에 표시.
- 삼항연산 사용가능 ``{a == true ? result1 : result2}``
- JSX내 인라인 스타일 사용가능(문법은 차이가 있음.)
    ``` html
    <!-- style 선언후 -->
    <div style={style}></div>
    <!-- 직접적용시 -->
    <div style={{backgroundColor:black}}></div>
    ```
- class``(.class)`` 속성시 ``className``사용

## 실행 순서
index.js -> 
app.js(최상위 리액트 화면 컴포넌트) -> 
하위 컴포넌트(개발한 ui컴포넌트) ->
index.html의 특정 태그내에(div id="root") 표시됨.

## yarn.lock
디펜던시 확인만 할것 수정금지.


## prettier
.prettierrc
```JSON
{
    "singleQuote": true,
    "semi":true,
    "useTabs":false,
    "tabWidth": 2
}
```
