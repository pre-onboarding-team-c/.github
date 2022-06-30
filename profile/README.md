<img width="1052" alt="스크린샷 2022-06-30 오후 9 01 47" src="https://user-images.githubusercontent.com/87293880/176672332-6fb6a0b9-b64f-4131-86ea-eb837f801b36.png">

## 소개 # 3기
|이름|팀|역할|깃허브|이메일|
|:----:|:----:|:---:|:----|:--|
|김지유|C|팀장|[@scvgood287](https://github.com/scvgood287)|kgeeeu@gmail.com|
|김영우|C|팀원|[@whoamixzerone](https://github.com/whoamixzerone)|whoamixzerone@gmail.com|
|황시우|C|팀원|[@nicesiu](https://github.com/nicesiu)|siuh0403@gmail.com|

---

## 환경
![node](https://img.shields.io/badge/node-v16.15.1-3776AB?&style=plastic&logo=JavaScript&logoColor=white?label=healthinesses)
![npm](https://img.shields.io/badge/npm-v8.13.1-7986cb?&style=plastic&logo=npm&logoColor=white?label=healthinesses)

---

## 컨벤션
### Git 컨벤션
>Git 브랜치 전략
- Issue 생성 및 담당자를 결정한다.
- Project에서 해당 담당자가 할 일을 진행중으로 변경한다.
- 기능 구현 시, Branch이름 / Issue고유번호로 브랜치 분기 후 작업한다. ex( feature/1 )
- 기능 완료 후 리뷰어, 프로젝트 등을 설정하고 Pull Request한다.
- 리뷰어들이 리뷰 완료 후 문제가 없을 시 develop 브랜치로 merge한다.
- develop 에서 테스트 후 문제 없으면 main 브랜치로 merge한다.
>Git 프로세스
```
git pull origin develop -> 현재 개발되고 있는 브랜치 pull
git branch -> 어떤 브랜치가 스위칭되어있는지 확인
git checkout {브랜치명} -> 기능 구현 브랜치명으로 스위칭
git add . -> 변경내용 추가
git commit -m “{매세지 내용}” -> Git 커밋 메세지 컨벤션에 따름
git push origin {브랜치명} -> 기능 구현한 것을 푸시
```
>Branch 이름

- main : 기준이 되는 브랜치로 제품을 배포하는 브랜치
- develop : 개발 브랜치로 개발자들이 이 브랜치를 기준으로 각자 작업한 기능들을 merge
- feature : 단위 기능을 개발하는 브랜치로 기능 개발이 완료되면 develop 브랜치에 merge

>Issue 생성
- Title : 간략한 기능 명칭
- Comment : 구체적인 기능 내용 설명
- Projects 설정
- Labels 용도에 맞게 설정
- 담당자 있을 시 Assigness 설정

>Commit 메세지 컨벤션
```
type : (아래 규율에 따름)
body : 최대 30자를 넘을 수 없으며, 구현한 내용을 한글로 작성한다.
footer : 선택사항이며 Issue 트래커 id로 사용이 된다.
```
type
- feat : 새로운 기능 추가
- fix : 버그 수정
- docs : 문서 수정
- style : 코드 포맷팅, 세미콜론 누락, 코드 변경이 없는 경우, linting
- refactor : 코드 리팩토링
- test : 테스트 코드, 리팩토링 테스트 코드 추가
- chore : 빌드 업무 수정, 패키지 매니저 수정

```
ex)
feat:로그인 구현#15
refactor:API구현 리팩토링
...
```
---
### Code 컨벤션
[Airbnb JavaScript 스타일 가이드 참조](https://github.com/tipjs/javascript-style-guide)
>주석
주석은 작성자명을 명시하고 아래와 같이 작성한다.
```
/**
 * 작성자 : 작성자명
 * A
 * B
 * C
 */

 ```
 >독스트링
 작성자를 명시하고 클래스나 함수 바로 위에 작성한다.
 ```
 /**
  * 작성자 : 작성자명
  * @param {파라미터1타입} 파라미터1 - 파라미터설명
  * @param {파라미터2타입} 파라미터2 - 파라미터2설명
  * @return {리턴타입} 리턴설명
  */
const f = (파라미터1, 파라미터2) => { return };
```
---
### 기타
>Repository 작성 규칙

PascalCase로 작성한다.
```
Repository명-C-회사이름
```
