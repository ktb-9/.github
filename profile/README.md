# 9조 - 테스구조


<div align="center">

<h1>Ripple Trip</h1>

<img src="https://github.com/ktb-9/.github/blob/main/readMeAsset/logo.png" height="300" alt="Reflective 로고">

<h3> "여행 일정을 쉽게 계획하고 가계부 및 사진 편집 앱 서비스" </h3>

<br />

<h2>직관적인 인터페이스로 여행 준비 완료</h2>

여행 일정을 손쉽게 계획하고, 가계부와 사진 편집까지 한 번에!  
직관적인 블록 에디터로 여행 준비의 모든 단계를 체계적으로 정리하고 공유하세요.  

여행 일정 계획, 사진 편집 및 공유, 여행 가계부 등록으로 더 편리하게 여행을 정산하고 준비할 수 있습니다.

</br>

[✨ < Ripple Trip > 트레일러](https://youtu.be/OwUcjOwQ9Gc)

</div>

<br />

# 목차

### [1. 프로젝트 소개](#%EF%B8%8F-프로젝트-소개)

- [< Ripple Trip >를 만들게 된 계기](#-Ripple-Trip-를-만들게-된-계기)
- [주요 기능 설명](#주요-기능-설명)
- [프로젝트 실행 방법](#프로젝트-실행-방법)

### [2. 기술 스택](#%EF%B8%8F-기술-스택)

### [3. 기술적 경험](#-기술적-경험)

- [FE](#FE)
  - [성능 최적화](#성능-최적화)
  - [FSD 아키텍처](#fsd-아키텍처)

<br />

# ⭐️ 프로젝트 소개

## < Ripple Trip >를 만들게 된 계기

여행 후 공동 지출을 정산할 때, 실생활에서 발생한 지출 항목과 여행 경비가 섞여 있어 이를 하나하나 찾아 나누는 일이 번거롭고 시간이 많이 소요되었습니다. 

이런 불편함을 겪으며, 더 효율적이고 간편한 여행 관리 방법을 고민하게 되었습니다. 

또한, 국내 여행을 더 쉽게 계획하고 준비할 수 있는 서비스의 필요성을 느꼈습니다. 여행 일정과 관련된 모든 요소를 하나의 플랫폼에서 관리할 수 있으면 여행 준비가 훨씬 더 수월하고 즐거운 경험이 될 것이라고 생각했습니다. 

그래서 여행 일정 관리에 초점을 맞추어, 여행을 계획하고 지출을 정산하며, 필요한 모든 정보를 직관적으로 제공할 수 있는 서비스를 구현하려 했습니다. 

이러한 고민과 아이디어를 바탕으로 **Ripple Trip**을 개발하게 되었습니다. 이 서비스는 여행 준비 과정에서 겪을 수 있는 불편함을 최소화하고, 여행을 더욱 편리하고 즐겁게 만들어 줄 것입니다.


<br />

## 주요 기능 설명

### [ 공동 일정 ]
 <img src="https://github.com/ktb-9/.github/blob/main/readMeAsset/%E1%84%80%E1%85%A9%E1%86%BC%E1%84%83%E1%85%A9%E1%86%BC%20%E1%84%8B%E1%85%B5%E1%86%AF%E1%84%8C%E1%85%A5%E1%86%BC.png" alt="블록에디터">
동행인 추가 버튼을 통해 링크를 공유하고, 동행자들과 함께 실시간으로 가능한 날짜를 조율하여 최종 여행 날짜를 확정합니다.

### [ 여행 일정 ]

<img src="https://github.com/ktb-9/.github/blob/main/readMeAsset/%E1%84%8B%E1%85%A7%E1%84%92%E1%85%A2%E1%86%BC%20%E1%84%8B%E1%85%B5%E1%86%AF%E1%84%8C%E1%85%A5%E1%86%BC.png" alt="글 작성 이미지">

여행 일정은 날짜별로 자유롭게 작성할 수 있으며, 원하는 장소와 시간을 손쉽게 추가할 수 있습니다. 
카카오 키워드 검색을 통해 간편하게 장소를 검색하고, 애플 지도 연동으로 편의성을 강화했습니다. 
생성된 일정은 그룹 멤버들과 공유하여 함께 여행 계획을 조율할 수 있습니다.

### [ 가계부 ]

<img src="https://github.com/ktb-9/.github/blob/main/readMeAsset/%E1%84%80%E1%85%A1%E1%84%80%E1%85%A8%E1%84%87%E1%85%AE.png" alt="메인 페이지">

여행 중 발생한 지출을 간편하게 가계부에 등록할 수 있습니다. 
지출명, 일자, 지출액을 입력한 후 결제자와 공동 지출자를 선택할 수 있습니다. 
공동 지출자로 선택된 동행인의 개인 가계부에 자동으로 반영되며, 
정산 금액과 상대방의 지출 내역이 명확히 표시되어 편리하게 정산을 진행할 수 있습니다.

### [ 여행 요약  ]

<img src="https://github.com/ktb-9/.github/blob/main/readMeAsset/%E1%84%8B%E1%85%A7%E1%84%92%E1%85%A2%E1%86%BC%20%E1%84%8B%E1%85%AD%E1%84%8B%E1%85%A3%E1%86%A8.png" alt="실시간 알림 시스템"/>

여행 종료 버튼을 클릭하면 여행 전체 요약을 확인할 수 있습니다. 
여기에는 여행 일정, 가계부, 소비 패턴 분석이 포함됩니다. 
DB 기반의 소비 패턴 분석을 통해 지출 항목에 대한 세부 계산이 가능하며, 사용자는 자신의 소비 성향을 명확히 파악할 수 있습니다. 
이를 통해 종합적인 여행 활동을 한눈에 확인하고, 향후 여행에 대한 유용한 인사이트를 얻을 수 있습니다.

### [ 사진 편집 ]

<img src="https://github.com/ktb-9/.github/blob/main/readMeAsset/%E1%84%89%E1%85%A1%E1%84%8C%E1%85%B5%E1%86%AB%20%E1%84%91%E1%85%A7%E1%86%AB%E1%84%8C%E1%85%B5%E1%86%B8.png" alt="글 검색">

여행 중 찍은 사진에서 많은 사람들이 있는 부분을 제거할 수 있는 객체 제거 기능이 제공됩니다. 
또한, 브러쉬 도구와 사각형 도구를 사용해 사진의 특정 영역을 선택하여 삭제 또는 프롬프트를 이용해 자동으로 객체를 생성할 수 있습니다.
업스케일링 기능을 통해 사진을 고해상도로 변환할 수 있는 기능도 제공됩니다. 
이를 통해 사용자는 더욱 편리하게 사진을 수정하고 향상시킬 수 있습니다.

<br />

## 프로젝트 실행 방법

```bash
pnpm install

pnpm dev
```

<br />

# ⚒️ 기술 스택

<img src="https://github.com/kwangyoulsagong/Reflective/blob/main/readmeAssets/skills.png" height="500" alt="기술스택 이미지"/>

![Reflective 시스템 아키텍처](https://github.com/ktb-9/.github/blob/main/readMeAsset/%E1%84%8B%E1%85%A1%E1%84%8F%E1%85%B5%E1%84%90%E1%85%A6%E1%86%A8%E1%84%8E%E1%85%A5.png)

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


