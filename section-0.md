## Node.js 이해 

### Node.js란 무엇인가?
Node.js는 Chrome V8 Javascript 엔진으로 빌드된 JavaScript가 통작하는 환경(런타임)입니다.

> Chrome V8 Javascript 엔진?
> 자바스크립트가 빨라지고, 이걸 기반으로 노드 js가 만들어진다.
> JavaScript 런타임?
> 자바스크립트가 동작할 수 있는 환경. 브라우저 이외의 다른곳에 동작할수 있는 runtime이 탄생

### 웹 브라우저 동작 과정
HTML, CSS, JS => 브라우저를 통해 랜더링 => 화면출력

HTML, CSS 는 브라우저 내의 렌더링 엔진을 통해서 해석
자바스크립트는 브라우저 내의 자바스크립트 엔진을 통해서 해석이 된다.

### Node.js 구조 
* Single Thread : 작업을 처리하는 곳이 하나
* Non-blocking I/O : 앞선 작업이 오래 걸릴 경우, 먼저 처리된 결과를 리턴

