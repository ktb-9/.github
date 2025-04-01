# 9조 - 테스구조


<div align="center">

<h1>Ripple Trip</h1>

<img src="https://github.com/ktb-9/.github/blob/main/readMeAsset/logo.png" height="30" alt="Reflective 로고">

<h3> "블록 에디터 기반으로 회고를 작성할 수 있는 블로그 서비스" </h3>

<br />

<h2>당신의 아이디어를 자유롭게 표현할 수 있는 공간</h2>

생각의 조각들을 블록으로 쌓아올리며 당신만의 이야기를 만들어보세요.

최적화된 블록 에디터로 글쓰기의 즐거움을 다시 발견하세요.

다양한 블록 타입으로 글, 이미지, 코드 등을 자유롭게 구성

직관적인 드래그 앤 드롭으로 콘텐츠 재배치

</br>

[✨ < Reflective > 사용해보기](https://reflective.site/)

</div>

<br />

# 목차

### [1. 프로젝트 소개](#%EF%B8%8F-프로젝트-소개)

- [< Reflective >를 만들게 된 계기](#-Reflective-를-만들게-된-계기)
- [주요 기능 설명](#주요-기능-설명)
- [프로젝트 실행 방법](#프로젝트-실행-방법)

### [2. 기술 스택](#%EF%B8%8F-기술-스택)

### [3. 기술적 경험](#-기술적-경험)

- [FE](#FE)
  - [성능 최적화](#성능-최적화)
  - [FSD 아키텍처](#fsd-아키텍처)

<br />

# ⭐️ 프로젝트 소개

## < Reflective >를 만들게 된 계기

블로그 서비스를 개발하면서 겪은 에디터 개발 과정을 공유하려고 합니다. 처음에는 많은 블로그들처럼 마크다운 에디터를 만들었습니다. 마크다운은 간단한 문법으로 글을 작성할 수 있어서 좋았지만 사용하다 보니 몇 가지 불편한 점이 있었습니다.

#### 마크다운의 한계

티스토리나 벨로그 같은 블로그를 사용해 봤다면 이런 불편함을 느껴봤을 겁니다:

- 마크다운 문법을 계속 기억해야 함: `#`, `*`, \`\`\` 같은 기호들을 계속 입력해야 하는 불편한 점이 있습니다.
- 작성하는 내용과 결과물이 다름: 왼쪽에는 마크다운, 오른쪽에는 미리보기... 계속 두 화면을 왔다 갔다 해야 했습니다.
- 목록이나 표 같은 복잡한 구조 만들기 어려움: 여러 단계의 목록을 만들 때 들여쓰기 계산하는 것이 까다로웠습니다.
- 코드 블록 외에 특별한 콘텐츠 넣기 어려움: 차트나 다이어그램 같은 요소를 삽입하려면 외부 서비스에서 이미지로 만들어 가져와야 했습니다.

#### 노션처럼 만들고 싶었습니다.

노션이나 미디엄 같은 서비스들은 블록 단위로 콘텐츠를 관리하는 방식이 정말 편리해 보였습니다. "내 블로그도 이렇게 만들면 어떨까?" 하는 생각이 들었죠. 그래서 우리는 블록 에디터 기반의 블로그 서비스, **Reflective**를 만들게 되었습니다.

<br />

## 주요 기능 설명

( gif 로딩이 느릴 수 있습니다🥹 조금만 기다려주세요 )

### [ 글 작성 ]

<table>
  <tr>
    <td><img src="https://assetkungya.s3.ap-northeast-2.amazonaws.com/%E1%84%82%E1%85%A1%E1%84%8B%E1%85%B4-%E1%84%83%E1%85%A9%E1%86%BC%E1%84%8B%E1%85%A7%E1%86%BC%E1%84%89%E1%85%A1%E1%86%BC-3.gif" alt="블록 에디터 1" /></td>
    <td><img src="https://assetkungya.s3.ap-northeast-2.amazonaws.com/%E1%84%82%E1%85%A1%E1%84%8B%E1%85%B4-%E1%84%83%E1%85%A9%E1%86%BC%E1%84%8B%E1%85%A7%E1%86%BC%E1%84%89%E1%85%A1%E1%86%BC-4.gif" alt="블록 에디터 2" /></td>
  </tr>

  <img src="https://github.com/kwangyoulsagong/Reflective/blob/main/readmeAssets/%EB%B8%94%EB%A1%9D%EC%97%90%EB%94%94%ED%84%B0.gif" alt="블록에디터">
</table

#### 1. **블록 기반 편집**

- 각 콘텐츠(문단, 이미지, 목록 등)를 블록 단위로 분리하여, 사용자가 자유롭게 콘텐츠를 삽입, 이동, 삭제할 수 있습니다.
- 이를 통해 직관적이고 유연한 글 작성이 가능합니다.

#### 2. **실시간 미리보기**

- 작성 중인 콘텐츠를 실시간으로 미리 볼 수 있어, 포스트의 레이아웃을 즉시 확인하고 수정할 수 있습니다.
- 글 작성과 동시에 포스트의 최종 형태를 시각적으로 확인할 수 있어 효율적인 작성이 가능합니다.

#### 3. **다양한 블록 타입**

- 텍스트, 이미지, 코드 블록, 목록 등 다양한 블록 타입을 제공하여, 사용자는 포스트의 내용에 맞는 다양한 형식으로 글을 작성할 수 있습니다.
- 또한, 차트를 삽입할 수 있는 기능을 제공하여, 데이터를 시각적으로 표현할 수 있습니다.

### [ 글 조회 ]

<img src="https://github.com/kwangyoulsagong/Reflective/blob/main/readmeAssets/%EA%B8%80%EC%A1%B0%ED%9A%8C.gif" alt="글 작성 이미지">

- 글은 블록 타입 형식으로 적용된 글을 볼 수 있습니다.
- 헤딩(Heading) 내비게이션을 통해 해당 헤딩으로 라우팅 지원합니다.

<img src="https://github.com/kwangyoulsagong/Reflective/blob/main/readmeAssets/%EB%8C%93%EA%B8%80%20%EB%8C%80%EB%8C%93%EA%B8%80.gif" alt="글 커스텀 이미지">

- 해당 게시물에 댓글을 달 수 있습니다.
- 답글도 지원해서 커뮤니티 활성화를 할 수 있습니다.

### [ 메인 페이지 ]

<img src="https://github.com/kwangyoulsagong/Reflective/blob/main/readmeAssets/%EB%A9%94%EC%9D%B8%ED%8E%98%EC%9D%B4%EC%A7%80.gif" alt="메인 페이지">

- Top 8 인기 게시물 최신 트렌드로 애니메이션 반영했습니다.
- 최근 게시물들을 좋아요 순으로 탑 3을 먼저 표시하고,
- 그 이후로는 최신 날짜 기준으로 정렬하는 방식으로 반영했습니다.

### [ 실시간 알림 시스템 ]

<img src="https://github.com/kwangyoulsagong/Reflective/blob/main/readmeAssets/%EC%95%8C%EB%A6%BC.gif" alt="실시간 알림 시스템"/>

- 실시간 알림을 통한 댓글, 좋아요, 즐겨찾기 이벤트 발생시 즉시 전송했습니다.

### [ 글 검색 ]

<img src="https://github.com/kwangyoulsagong/Reflective/blob/main/readmeAssets/%EA%B2%80%EC%83%89.gif" alt="글 검색">

- 검색은 제목 또는 작성자로 검색할 수 있습니다.
- 검색해서 해당 블로그로 이동할 수 있습니다..

<br />

## 프로젝트 실행 방법

```bash
pnpm install

pnpm dev
```

<br />

# ⚒️ 기술 스택

<img src="https://github.com/kwangyoulsagong/Reflective/blob/main/readmeAssets/skills.png" height="500" alt="기술스택 이미지"/>

![Reflective 시스템 아키텍처](https://assetkungya.s3.ap-northeast-2.amazonaws.com/reflective.png)

# 💪🏻 기술적 경험

## FE

프론트엔드의 주요 기술적 도전은 블록 에디터를 구현하는 것이었습니다. 기존의 마크다운 에디터와는 달리, 블록 에디터는 각 콘텐츠 요소(텍스트, 이미지, 코드 등)를 독립적인 '블록'으로 다루어 더 직관적이고 유연한 편집 경험을 제공합니다.

먼저 아래는 블록 에디터 구현 과정입니다.

- [마크다운에서 블록 에디터로: 내 블로그 에디터 개발기](https://velog.io/@tkrhdrhkdduf/%EB%A7%88%ED%81%AC%EB%8B%A4%EC%9A%B4%EC%97%90%EC%84%9C-%EB%B8%94%EB%A1%9D-%EC%97%90%EB%94%94%ED%84%B0%EB%A1%9C-%EB%82%B4-%EB%B8%94%EB%A1%9C%EA%B7%B8-%EC%97%90%EB%94%94%ED%84%B0-%EA%B0%9C%EB%B0%9C%EA%B8%B0)

- [메인 페이지 최근 게시물 UX 개선 (가상 스크롤)](https://velog.io/@tkrhdrhkdduf/%EA%B0%80%EC%83%81-%EC%8A%A4%ED%81%AC%EB%A1%A4-Virtual-Scroll-%EA%B5%AC%ED%98%84)

<br />

### 성능 최적화

- [블록 에디터 성능 개선](https://velog.io/@tkrhdrhkdduf/%EB%B8%94%EB%A1%9D-%EC%97%90%EB%94%94%ED%84%B0-%EC%84%B1%EB%8A%A5-%EA%B0%9C%EC%84%A0)

처음 블록 에디터를 개발했을 때, 몇 가지 심각한 성능 문제가 있었습니다:

- 텍스트 입력할 때마다 화면이 버벅였습니다.
- 블록이 많아질수록 에디터가 느려졌습니다.
- 메모리 사용량이 계속 증가했습니다.
- 초기 로딩이 느렸습니다.

---

#### 1. React의 렌더링 개선 기법 적용

제가 선택한 첫 번째 최적화 방식은 **React의 렌더링 개선 기법**을 적용하는 것이었습니다.  
React의 렌더링 사이클은 크게 **렌더 페이즈**와 **커밋 페이즈**로 구성됩니다.  
불필요한 렌더 페이즈를 줄이기 위해 `React.memo`, `useMemo`, `useCallback`과 같은 기법을 적용했습니다.  
특히 `BlockEditor` 컴포넌트에 `React.memo`를 적용하여 **특정 블록만 변경되었을 때 해당 블록만 리렌더링**되도록 개선했습니다.

하지만 이런 기본적인 최적화만으로는 충분하지 않았고,  
특히 문서 크기가 커질수록 여전히 성능 저하가 발생했습니다.

---

#### 2. Map 자료구조를 활용한 상태 관리 개선

추가적인 최적화를 위해 **블록 데이터 관리 방식을 변경**했습니다.  
기존에는 **배열 기반**으로 블록 상태를 관리했는데, 이 방식은  
하나의 블록이 변경될 때마다 전체 배열이 갱신되어 **모든 블록이 리렌더링**되는 문제가 있었습니다.  
이를 해결하기 위해 **Map 자료구조**를 도입했습니다.

#### 3. 디바운싱을 통한 입력 최적화

마지막으로 적용한 최적화는 사용자 입력에 대한 디바운싱 처리였습니다.
초기에는 모든 키 입력마다 상태를 업데이트했고,
이로 인해 과도한 렌더링과 성능 저하가 발생했습니다.

이를 해결하기 위해 lodash의 debounce 함수를 사용하여
300ms 지연 시간을 설정, 연속된 입력을 하나의 업데이트로 처리했습니다.

<table>
  <tr>
    <td><img src="https://velog.velcdn.com/images/tkrhdrhkdduf/post/50919b5d-41e1-4055-b723-cfd532f28d5d/image.png" alt="블록 에디터 1" /></td>
    <td><img src="https://velog.velcdn.com/images/tkrhdrhkdduf/post/e9375921-e6ed-49f0-8e6f-732e16291fda/image.png" alt="블록 에디터 2" /></td>
  </tr>
</table

<table>
  <tr>
    <td><img src="https://velog.velcdn.com/images/tkrhdrhkdduf/post/6060341a-1af9-4768-8bd5-c07eaec8cd22/image.png" alt="블록 에디터 1" /></td>
    <td><img src="https://velog.velcdn.com/images/tkrhdrhkdduf/post/9efc3d54-a6be-4354-9e4d-415a8880db15/image.png" alt="블록 에디터 2" /></td>
  </tr>
</table>



### 팀 프로젝트 문서
[![Team Notion](https://img.shields.io/badge/TEAM_Notion-000000?style=for-the-badge&logo=notion&logoColor=white)](https://goormkdx.notion.site/9-d30dfb6a9fd64bfdb2f278a0f4965b68)


## 파트 구성

### Full Stack

사용 기술 스택

[![ReactNative](https://img.shields.io/badge/ReactNative-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://reactnative.dev/)
[![SpringKotlin](https://img.shields.io/badge/Spring+Kotlin-000000?style=for-the-badge&logo=spring&logoColor=green)](https://spring.io/)

<div align="center">
  
| **Hardy** | **Ten** | 
| :------: |  :------: | 
| <img src="https://github.com/ktb-9/.github/blob/main/profile/image/hardy.png?raw=true" height=150 width=150> <br/>  [![hardy github](https://img.shields.io/badge/Hardy-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/kwangyoulsagong)| <img src="https://github.com/ktb-9/.github/blob/main/profile/image/ten.png?raw=true" height=150 width=150> <br/> [![ten github](https://img.shields.io/badge/ten-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/yeollow) |

</div>

### Cloud

**사용 기술 스택**

[![Kubernetes](https://img.shields.io/badge/Kubernetes-2496ED?style=for-the-badge&logo=kubernetes&logoColor=white)](https://kubernetes.io/ko/)
[![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon-aws&logoColor=white)](https://aws.amazon.com/)

<div align="center">
  
| **Zoey** | **Lucy** | 
| :------: |  :------: | 
| <img src="https://github.com/ktb-9/.github/blob/main/profile/image/zoey.png?raw=true" height=150 width=150> <br/>  [![zoey github](https://img.shields.io/badge/zoey-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ChoiYoo)| <img src="https://github.com/ktb-9/.github/blob/main/profile/image/lucy.png?raw=true" height=150 width=150> <br/> [![lucy github](https://img.shields.io/badge/lucy-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/iyxxnjin) |

</div>

### AI
사용 기술 스택

[![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)](https://www.tensorflow.org/)
[![Flask](https://img.shields.io/badge/Flask-000000?style=for-the-badge&logo=flask&logoColor=white)](https://flask.palletsprojects.com/)

<div align="center">
  
| **Kyle** | **Juyeon** | 
| :------: |  :------: | 
| <img src="https://github.com/ktb-9/.github/blob/main/profile/image/kyle.png?raw=true" height=150 width=150> <br/>  [![kyle github](https://img.shields.io/badge/kyle-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/KDK-00)| <img src="https://github.com/ktb-9/.github/blob/main/profile/image/juyeon.png?raw=true" height=150 width=150> <br/> [![juyeon github](https://img.shields.io/badge/juyeon-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/juyeonbae) |

</div>

## 저희 팀은 이렇게 일해요

### 커뮤니케이션
- Discord, Notion, Github를 사용하여 의사소통합니다.
- Discord를 통해 공지사항 전달, 지식 공유, 회의 진행, 질의, 요청사항 건의를 진행합니다.
- Notion을 통해 회의록 관리 및 미션, 스터디 관련 문서를 정리합니다.
- Github를 통해 일정 관리, 코드 리뷰, 프로젝트 관련 문서 정리를 진행합니다.
- 정기 회의는 수요일 14시에 Discord에서 진행합니다.
- 추가 회의가 필요한 경우 Discord 내 요청하기를 통해 요청합니다.

### 스프린트 규칙
- 배포 가능한 최소 단위로 스프린트를 계획합니다.

### 워크 플로우
1. 스프린트 단위로 Github에 프로젝트, 마일스톤을 생성합니다.
2. 해당 프로젝트에 기능 작업 단위로 이슈를 등록합니다.
3. 이슈 내용에 맞춰 개발을 진행합니다.
4. 기능 작업 단위의 개발이 완료된 경우 PR을 생성합니다.
5. 코드 리뷰 규칙에 맞춰 리뷰를 진행합니다.
6. 모든 conversation이 해결된 경우 merge를 진행합니다.
7. 스프린트 내 모든 이슈가 해결되거나 스프린트 기간이 종료된 경우 회고를 진행합니다.

### 회고 방식
- 회고는 한 단위의 스프린트가 종료된 시점에 진행합니다.
- 개별 회고록을 작성합니다.
- 개별 회고록을 기반으로 회고록 공유회를 진행합니다.
- 공유회를 통해 이후 스프린트에 반영 할 사항은 정립합니다.

### 스터디 방식
- Discord를 요청 채널을 통해 스터디를 제안합니다.
- 2명 이상이 모인 경우 스터디를 진행합니다.
- 스터디는 가능하면 비동기적으로 진행합니다.
- Github와 Notion을 통해 스터디 내용을 정리합니다.


