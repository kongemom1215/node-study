# 1강 : Node JS 란?
## Node.js 이해 
https://www.youtube.com/watch?v=pK2IKP3M5Ls&t=2s

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

### Node.js 특징
#### 구조 
* Single Thread : 작업을 처리하는 곳이 하나
* Non-blocking I/O : 앞선 작업이 오래 걸릴 경우, 먼저 처리된 결과를 리턴

![image](https://github.com/user-attachments/assets/9234b5cf-bd4b-4c5f-9d45-a95f9b811e14)

Libuv 라는 라이브러리가 Non-blocking I/O를 가능하게 해준다.
라이브러리 내부 프로세스는 오래걸리는작업, 일반 작업을 분리를 시켜서 각각 요청을 보내고, 먼저 끝내는 것들을 event loop를 통해서 돌려준다.

#### 확장성
개발 환경에서 프로젝트 자체 확장을 쉽게 할 수 있다.  
**어떻게?**  
Node JS에서 제공하는 `NPM(Node Package Manager)`라는 툴 덕분  

다양한 내부, 외부 묘듈(패키지)가 제공됨 => 필요한 기능들이 미리 구현되어 있는 경우가 많음

> Node js 개발을 도와주는 nvm, npx, yarn 등 다양한 툴 사용 가능  
> nvm(Node Version Manager) : 특정 버전의 Node.js를 설치하기 위한 툴  
> npx :  npm을 관리하기 위한 모듈  
> yarn : 페이스북에서 만든 패키지 툴 (npm과 같은 기능을 수행)
