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
  - [문제 및 해결](#문제-및-해결)
- [BE](#BE)
  - [서버 발생한 문제들](#서버-문제-및-해결)


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

<img src="https://github.com/ktb-9/.github/blob/main/readMeAsset/%E1%84%80%E1%85%B5%E1%84%89%E1%85%AE%E1%86%AF%E1%84%89%E1%85%B3%E1%84%90%E1%85%A2%E1%86%A8.png" height="500" alt="기술스택 이미지"/>

![Reflective 시스템 아키텍처](https://github.com/ktb-9/.github/blob/main/readMeAsset/%E1%84%8B%E1%85%A1%E1%84%8F%E1%85%B5%E1%84%90%E1%85%A6%E1%86%A8%E1%84%8E%E1%85%A5.png)

# 💪🏻 기술적 경험

## FE

프론트엔드의 주요 기술적 도전은 리액트 네이티브와 웹소켓을 활용한 실시간 공동 일정 관리 기능을 구현하는 것이었습니다. <br />
특히, 리액트 네이티브를 사용하여 모바일 환경에서의 사용자 경험을 최적화하고, 웹소켓을 통해 동행자들과 실시간으로 일정을 조율하는 기능을 구현했습니다. <br />
또한, `SSR(서버사이드 렌더링)`을 적용한 Next.js를 사용하여 웹뷰를 바탕으로 이밎 브러쉬 와 같은 기능을 처음으로 구현하며, <br />
캔버스 기반의 이미지 편집 기능을 추가하여 사용자들이 사진을 편집하고, 원하는 부분을 수정할 수 있도록 했습니다.

먼저 아래는 이미지 편집 기능 과정입니다.
- [캔버스-기반-다중-레이어-이미지-편집기-구현하기](https://velog.io/@tkrhdrhkdduf/%EC%BA%94%EB%B2%84%EC%8A%A4-%EA%B8%B0%EB%B0%98-%EB%8B%A4%EC%A4%91-%EB%A0%88%EC%9D%B4%EC%96%B4-%EC%9D%B4%EB%AF%B8%EC%A7%80-%ED%8E%B8%EC%A7%91%EA%B8%B0-%EA%B5%AC%ED%98%84%ED%95%98%EA%B8%B0)

<br />

### 문제 및 해결

- [실시간 공동 일정 작성 문제 해결](https://velog.io/@tkrhdrhkdduf/%EC%8B%A4%EC%8B%9C%EA%B0%84-%EA%B3%B5%EB%8F%99-%EC%9D%BC%EC%A0%95-%EC%9E%91%EC%84%B1-%EB%AC%B8%EC%A0%9C-%ED%95%B4%EA%B2%B0)

# Socket.io 실시간 기능 구현 시 문제점과 해결 과정

## 발생한 문제들

### 1. 앱 백그라운드 전환 시 연결 불안정 문제
사용자가 앱을 잠시 나갔다 돌아오면 소켓 연결이 끊어져 데이터가 사라지거나 변경사항이 반영되지 않음  
모바일 환경에서 특히 심각 (백그라운드 전환 시 자원 절약을 위해 연결 종료)  
"여행 일정을 친구와 함께 짜다가 잠깐 카톡 확인하고 돌아왔더니 내가 작성하던 일정이 모두 사라져 있어요!" - 테스터 피드백

### 2. 그룹 멤버 관련 동기화 문제
그룹에서 나간 사용자가 여전히 멤버로 표시되는 문제  
삭제된 그룹에 일부 사용자가 계속 접근 가능한 문제  
"그룹에서 나갔는데도 계속 멤버로 표시되네요?" - 테스터 피드백

### 3. 일정 데이터 동기화 문제
퇴장한 멤버의 일정 데이터가 계속 남아있는 문제  
동시 수정 시 변경사항이 실시간으로 정확히 반영되지 않는 문제  
"퇴장한 멤버가 작성한 일정이 왜 아직도 보이죠?" - 테스터 피드백

## 해결책 고민 과정

### 1. 연결 안정성 문제
#### 초기 접근:
- 사용자에게 '새로고침' 버튼 제공 → 사용자 경험 저하로 기각

#### 고민했던 옵션:
- **전송 방식**: WebSocket만 사용 vs 기본값(WebSocket + HTTP Long Polling)
- **자동 재연결 전략**: 재시도 빈도와 기간
- 앱 생명주기 이벤트(포그라운드/백그라운드 전환) 활용 방법

#### 결론:
- WebSocket만 사용하는 것이 모바일 환경에서 더 안정적, 자동 재연결 기능 필수

### 2. 그룹 멤버 동기화 문제
#### 고민했던 방법:
- 클라이언트에서 멤버 상태 관리 + 주기적 서버 동기화
- 서버를 단일 진실 공급원(single source of truth)으로 활용
- 모든 상황을 커버할 이벤트 정의

#### 결론:
- 서버를 단일 진실 공급원으로 사용, 명확한 이벤트 시스템 구축

### 3. 일정 데이터 동기화 문제
#### 고민했던 방법:
- 멤버 퇴장 시 작성 일정 자동 삭제 vs 일정 유지 + 작성자 정보 변경
- 실시간 동기화를 위한 최적 이벤트 구조

#### 결론:
- 팀 내 의견 분분, 사용자 테스트를 통해 최적안 도출

## 최종 해결책

### 1. 연결 안정성 강화
- WebSocket만 사용하도록 설정하여 전송 방식 전환으로 인한 불안정 해소
- 자동 재연결 기능으로 사용자 개입 없이 연결 복구
- 연결 오류 시 명확한 피드백 제공
- 앱 포그라운드 복귀 시 연결 상태 확인 및 데이터 재동기화

### 2. 그룹 멤버 관리 개선
- 서버 발생 그룹 관련 이벤트(삭제, 멤버 퇴장)를 클라이언트에서 적절히 처리
- 소켓 연결 직후 최신 멤버 정보 요청하여 항상 최신 상태 유지

### 3. 일정 데이터 동기화 개선
- 핵심 이벤트 구현: 초기 데이터 로드, 일정 업데이트, 일정 삭제
- 컴포넌트 언마운트 시 이벤트 리스너 제거 및 소켓 연결 종료로 리소스 관리

이러한 개선을 통해 실시간 협업 기능의 안정성과 사용자 경험을 크게 향상시켰습니다.

## BE

### 서버 문제 및 해결

### 발생한 문제들

### 1. 심각한 동시성 이슈
- 여러 사용자가 동시에 여행 일정, 경비 정보, 결제 정보, 위치 데이터에 접근할 때 문제 발생
- 여러 테이블 간 교차 트랜잭션으로 인한 대기 상태 증가
- 서비스 응답 지연 및 사용자 경험 저하
- 데이터 수정 시 덮어쓰기 및 불일치 현상 발생
- 데드락 빈번하게 발생

## 해결책 고민 과정

### 1. 락(Lock) 전략 선택 고민
- **비관적 락(Pessimistic Lock)**과 **낙관적 락(Optimistic Lock)** 중 어떤 방식을 적용할지 고민
- 모든 데이터에 동일한 락 전략 적용 vs 데이터 특성에 따른 차별화된 락 적용
- 트랜잭션 시점에 따른 락 획득 전략 검토
- 데이터 일관성과 성능 사이의 균형점 모색

### 2. 데드락 처리 방안
- **데드락 발생 시** 단순 재시도 vs 지능적 재시도 전략
- 데드락 근본 원인 해결 방법 모색
- 데드락 발생 시 사용자 경험 개선 방안 검토
- 테이블 접근 순서 표준화의 실현 가능성 평가

### 3. 성능과 정확성 균형
- **완벽한 데이터 일관성 보장** vs **최고의 성능 추구**
- 트랜잭션 처리량 증가에 따른 시스템 안정성 영향 평가
- 사용자 경험 저하 없이 동시성 문제를 해결할 최적의 방법 탐색

## 최종 해결책

### 1. 데이터 특성에 맞는 락 전략 차별화
- **결제/정산 데이터**: 비관적 락(FOR UPDATE) 적용
  - 금융 정보는 절대적 정확성이 요구되므로 강력한 락으로 동시 접근 차단
  - 트랜잭션 시작 시 즉시 락 획득으로 데이터 일관성 100% 보장

- **여행 일정 데이터**: 버전 기반 낙관적 락 구현
  - 충돌 가능성이 상대적으로 낮은 일정 수정에는 버전 필드 추가
  - 충돌 발생 시에만 롤백하여 불필요한 락 대기 시간 감소

### 2. 지능적 데드락 처리 시스템 개발
- **MySQL 데드락 에러코드(1213)** 자동 감지 메커니즘 구현
- 최대 3회까지 점진적 대기 시간 증가 적용 (50ms→100ms→200ms)
- 일관된 테이블 접근 순서 표준화 (알파벳 순)로 교착상태 원천 차단
- 데드락 발생 로깅 및 분석 시스템 구축

### 3. 성능 최적화 조치
- 트랜잭션 격리 수준 최적화로 불필요한 블로킹 감소
- 인덱스 재구성으로 락 범위 최소화
- 트랜잭션 내 작업량 최소화로 락 유지 시간 단축
- 배치 처리 방식 도입으로 트랜잭션 처리량 향상

## 성과
- 동시 사용자 10명 이상 접속 시에도 데이터 정합성 100% 유지
- 초당 트랜잭션 처리량 10건에서 140건으로 14배 향상
- 데드락 발생률 95%에서 5%로 감소하여 안정적 서비스 제공
- 트랜잭션 성공률 20%에서 95% 이상으로 대폭 개선

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


