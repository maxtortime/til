# Rendering Elements
- React 공식 문서의 https://facebook.github.io/react/docs/rendering-elements.html 을 요약했습니다.

## 개요
- Elements는 React 앱을 궝하는 가장 작은 단위다.
- 브라우저의 DOM elements와 달리 React elements는 오브젝트다. 
- `Element`와 `Component`를 헷갈릴 수 있음.

## Element 렌더링 및 업데이트하기
- React Element를 렌더링하려면 `ReactDOM.render()`를 사용해야 함
- React Element는 immutable하므로 생성 후에 자식이나 속성을 바꿀 수 없다. 그러므로 UI를 업데이트 하는 유일한 방법은 Element를 새로 만들어서 렌더링하는 것 뿐이다.
- 일반적으로 `ReactDOM.render()`은 한 번만 호출되고 React에서 이전과 현재 element를 비교해서 필요한 부분만 업데이트한다.