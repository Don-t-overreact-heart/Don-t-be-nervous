- **CORS의 개념 및 해결방안**

  - **CORS 란?**

    우선 CORS란 Cross-Origin Resource Sharing으로 **교차(다른) 출처 리소스 공유**이다.

    CORS는 서로 다른 출처 간에 리소스를 전달하는 방식을 제어하는 체제.

    출처가 서로 같다고 판단하는 로직 자체는 굉장히 간단하다.두 URL 구성 요소 중 Scheme, Host, Port, 이 3가지만 동일하면 된다.

    ex) [https://evan-moon.github.io:80](https://evan-moon.github.io:80/)

    - scheme : https://
    - host : even-moon.github.io
    - port : :80이것만 같다면 나머지는 전부 다르더라도 같은 출처로 인정이된다.

    CORS 요청이 가능 하려면 서버에서 특정 헤더인 Access-Control-ALlow-Origin과 함께 응답할 필요가 있다.

  - **CORS 해결방법**

    웹 프론트 측에서 request header에 CORS 관련 옵션을 넣어주고, 서버에서는 해당 프론트 요청을 허용하면 됨

- **프런트엔드 성능 최적화 경험**

  위코드 기간 중 프로젝트를 하며 성능최적화를 했던 경험은 같은 스타일을 가진 컴포넌트를 재사용하여 코드를 줄이고 일부 이미지들을 크기가 더 작은 jpg, jpeg 를 주로 사용하는 방향으로 최적화한 경험이 있습니다.

  [https://velog.io/@deli-ght/웹-성능-최적화1](https://velog.io/@deli-ght/%EC%9B%B9-%EC%84%B1%EB%8A%A5-%EC%B5%9C%EC%A0%81%ED%99%941)

- **브라우저 동작 원리**

- **웹 서비스 배포 시스템 구축 경험**

  - **배포 경험에 대해서**

    비바이노베이션 인턴 시절 사수께서 CI/CD 를 설명하며 yml 파일을 만들고 AWS 를 활용하여 배포하시는 모습을 옆에서 지켜봤습니다. 직접 한게 아니며 옆에서 단순히 본 것 이기 때문에 해본 적이 없습니다.

  - **CI, CD가 무엇인지 아는지?**

    애플리케이션 개발단계를 자동화 하여 애플리케이션을 보다 짧은 주기로 고객에게 제공하는 방법.

    **기본 개념**

    - 지속적인 통합
    - 지속적인 서비스 제공
    - 지속적인 배포

    애플리케이션의 통합 및 테스트 단계에서부터 제공 및 배포에 이르는 애플리케이션의 라이프사이클 전체에 걸쳐 **지속적인 자동화와 지속적인 모니터링을 제공**.

    이런 구축 사례를 일반적으로 "CI/CD 파이프라인"이라 부르며 개발및 운영팀의 애자일방식을 통해 지원된다.

- 반응형 vs 적응형 웹 차이

  적응형 웹은 서버나 클라이언트에서 웹에 접근한 디바이스를 체크하여 그 다바이스에 최적화된 마크업을 호출한다.

  적응형 웹의 특징으로는 기존의 사이트를 재구축할 필요가 없고 다양한 디바이스에 최적의 성능을 가져올 수 있다.

  반면,

  반응형 웹은 미디어 쿼리를 사용하여 화면의 크기를 확인하고 유연한 이미지와 그리드로 화면 크기의 변화에 따라 그에 맞는 크기가 된다.

- 프로그레시브 렌더링 (Progressive rendering)

  프로그레시브 렌더링은 서버에서 웹페이지 일부를 순차적으로 렌더링하면서 전체 페이지가 렌더링 될 때까지 기다리지 않고 웹 페이지를 클라이언트에 스트리밍하는 기술입니다.
  즉, 콘텐츠를 가능한 빠르게 표시하기 위해 사용됩니다.

  점진적 렌더링은 서버에서 중요한 컨텐츠를 렌더링 한 후에 중요 하지 않은 콘텐츠를 기다리지 않고 클라이언트로 스트리밍을 시작 하는 기술입니다.

### 🔸 마케팅에서 중요한 데이터란

[데이터는 마케팅의 가장,행동 예측 등도 가능하다](https://www.dailysecu.com/news/articleView.html?idxno=122287#:~:text=%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%8A%94%20%EB%A7%88%EC%BC%80%ED%8C%85%EC%9D%98%20%EA%B0%80%EC%9E%A5,%ED%96%89%EB%8F%99%20%EC%98%88%EC%B8%A1%20%EB%93%B1%EB%8F%84%20%EA%B0%80%EB%8A%A5%ED%95%98%EB%8B%A4).

[CRM 마케팅에서 중요한 데이터와 지표 10가지](http://www.openads.co.kr/content/contentDetail?contsId=6739)

### 🔸 자료구조의 종류

자료구조 : 대량의 데이터를 효율적으로 관리할 수 있는 데이터의 구조를 의미. 어떤 데이터 구조를 사용하느냐에 따라 코드의 효율이 달라질 수 있다.

![](https://i.imgur.com/De3X1ra.png)

**선형구조** : 데이터들이 일렬로 쭉 저장되어 있는 형태

- List : 데이터를 나열하고, 각 데이터를 인덱스에 대응하도록 구성한 데이터 구조
- Queue : 줄을 서는 행위와 비슷한 구조로, 가장 먼저 넣은 데이터를 가장 먼저 꺼낼 수 있는 구조(FIFO, LILO)
- Stack : 데이터를 제한적으로 접근할 수 있는 구조로, 한쪽 끝에서만 자료를 넣거나 뺄 수 있어서 가장 나중에 쌓은 데이터를 가장 먼저 빼낼 수 있는 데이터 구조(LIFO, FILO)
- Deque : 양쪽 끝에서 자료의 삽입과 삭제가 모두 가능한 구조
- Linked List : 연결 리스트, 떨어진 곳에 존재하는 데이터를 화살표로 연결해서 관리하는 데이터 구조

**비선형구조** : 데이터가 트리 형태로 저장되어 있다고 생각하고 사용하는 자료구조

- Graph : node(노드)/vertex(정점) 사이에 edge(엣지)가 있는 구조
  - node/vertex : 위치
  - edge(link, branch) : 위치 간의 관계를 표시한 선, 노드를 연결한 선
  - 종류 : 무방향 그래프, 방향 그래프, 가중치/네트워크 그래프, 연결 그래프, 비연결 그래프, 사이클그래프, 비순환 그래프, 완전 그래프
- Tree : node로 구성된 계층적 자료구조, 트리는 그래프의 한 종류이다.
- 그래프와 트리의 차이점

![](https://i.imgur.com/myGw80R.png)

> [prepare_frontend_interview/Data_Structure.md](https://github.com/junh0328/prepare_frontend_interview/blob/main/Data_Structure.md)

- **트리가 무엇인지 구조 설명**

  - 루트 노드가 존재하며, 각각의 노드들은 루트 아래로 부속 트리를 이루며 순환 구조를 띠지 않는 비선형 자료구조를 트리라고 합니다.

- **트리 구조를 어떤 기능 개발에 응용할 수 있을지**

  - 트리의 주 목적은 탐색으로 검색 엔진, DBMS, 파일시스템, 라우터 알고리즘 등에서 사용됩니다.
