# Introducing JSX
- https://facebook.github.io/react/docs/introducing-jsx.html 내용 요약

## 개요
```js
const element = <h1>Hello, world!</h1>;
```
- 위 구문은 문자열도 HTML도 아닌 JSX라고 함
- JSX는 React `elements`를 생성하며 DOM 렌더링에 이용됨

## JSX 안에 JS 표현식 쓰기
- JSX안에 어떤 JS 표현식도 사용할 수 있음
- JSX를 여러 줄로 나눌 수 있지만 [자동 세미콜론 삽입](http://stackoverflow.com/q/2846283)을 방지하기 위해서 괄호를 치는 것이 좋음.
- JSX 자체가 컴파일 과정에서 JS 오브젝트가 되므로 제어문, 변수에 배정, 인수 및 반환값으로 모두 쓸 수 있다.

## JSX의 속성 지정하기
- JSX 속의 태그 속성을 지정할 수 있음
- 역시 중괄호를 써서 js 표현식으로 속성을 정의할 수 있음.
- 다만 JSX 속성을 만들 때 따옴표로 감싸면 안 됨. 오직 문자열일때만 따옴표로 감싸고 표현식일때는 중괄호를 쓸 것.
- 둘 모두를 같은 속성에 사용하면 안 됨.

## JSX 의 children 명시하기
- 태그 안이 빈 경우 XML처럼 `>/` 로 닫아주면 된다.
- JSX 태그는 자식을 가질 수 있다.
- JSX는 HTML보다 JS에 가깝기 때문에 camelCase 네이밍을 하는 게 좋음.

## XSS 공격 예방 및 오브젝트 표현
- JSX에 작성된 내용은 렌더링 되기전에 모두 문자열로 변환되기 때문에 공격을 예방할 수 있음
- JSX 는 Babel이 `React.createElement()`로 컴파일 함
- `React.createElement()` 버그를 막아주는 몇가지 기능을 갖추고 있음
- 이렇게 작성된 JSX는 `React elements`가 되어 DOM을 만들게 된다
