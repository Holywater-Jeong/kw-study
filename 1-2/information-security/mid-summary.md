# 1주차. 정보보안 개요

## 보안공격의 이해 및 필요지식

- OS: 운영체제 사소한 약점부터 시작하여 보안 취약점을 노리기에 OS 지식 필요
- 네트워크: 기업 외부에서 공격하는 경우 주로 네트워크를 타고 들어와서 공격, 이를 이해하기 위해 필요
- 서버: 공격 대상이 되는 서버가 어떤 서비스를 제공하고 어떤 방식에 의해 동작되는지 알아야 공격으로부터 수비하는 방법 알 수 있음.
- 프로그래밍: 악성코드, 바이러스, 웜과 같은 해킹 프로그램에 대응하려면 프로그래밍의 기본적인 지식 필요

## 보안 모델과 솔루션

#### 보안의 3대 요소

- 기밀성
  - 정보를 오직 인가된 사용자에게만 허락
- 무결성
  - 부적절한 정보의 변경이나 파기 없이 정확하고 완전하게 보존된 것
  - 무결성 구성의 3가지 세부 요소
    - 정확성: 틀린내용 X
    - 완전성: 내용 중에 빠짐 X
    - 일관성: 다른 정보와 일치해야
- 가용성
  - 시기적절하면서 신뢰할 수 있는 정보로의 접근과 사용

#### 최근의 보안 추세

기밀성보다 무결성, 무결성보다 가용성이 더 큰 관심.

#### 보안 공격 대비책

- 기밀성
  - 외부에서 내부로 네트워크 접근 차단하는 정책 적용
  - 강한 인증을 위한 혼합 인증
  - PC를 끄고 퇴근하는 보안 정책 적용
- 무결성
  - 악성코드 탐지 및 차단 솔루션의 사용
  - 비승인 SW 사용 금지 보안 정책 적용
  - 비승인 SW 설치 금지하는 보안 솔루션 적용
- 가용성
  - 백업 솔루션의 사용으로 서비스 복구

## 보안 거버넌스

조직이 자신에게 적합한 보안 정책을 수립하고 수립된 보안 정책에 의해 보안 관련 조직을 구성하여 일련의 보안 활동을 수행하는 것.

#### APT(Advanced Persistent Threat) 공격

지능적 지속 위협: 오랜 잠복기간 동안 흔적을 남기지 않고 보안 취약점 정보를 수집하다가 수집된 정보를 악용하여 특정 시점에 보안 사고를 일으키는 공격

#### APT 공격 대비책

보안 거버넌스에 의한 관리

> 절차적 기술적 보안 모두 신경써야

# 2주차

#### 정보의 의미

- 법률적: 특정 목적을 위해 광 또는 전자적 방식으로 처리되어 부호, 문자, 음성, 음향 및 영상 등으로 표현된 모든 종류의 자료 또는 지식
- 사전적: 관찰이나 측정을 통하여 수집한 자료를 실제 문제에 도움이 될 수 있도록 정리한 지식 또는 그 자료
- 자료를 일정한 처리 과정을 통해 의사결정 과정에 유용하게 이용될 수 있도록 변환한 것으로 생산 또는 입수를 통해 컴퓨터나 정보저장 매체 등에 전자문서 형태로 기록되어 있는 것
- 가치 지향적이고 관심이 있는 사람들의 의사결정에 영향을 주면수 어느 정도 이익을 제공할 수 있는 자료이어야함.
- 일정한 의도를 가지고 정리해 놓은 자료의 집합, 정보가 되기 위해서는 이용자, 즉 어떤 목적을 갖는 사람이 있어야 하고 자료가 처리되어야 함.

#### 정보보호의 정의

- 정보의 훼손, 변조, 유출 등을 방지하기 위한 관리적.기술적 수단 마련하는 것.

#### 정보보호 대상

- 하드웨어(장비, 단말장비 등)
- 소프트웨어
- 데이터
- 네트워크
- 문서
- 인적요소

#### 정보보호의 기본 목표

- 정보보호의 요구사항이(`기밀성`, `무결성`, `가용성`) 곧 목표.
- 내부 또는 외부의 침입자나 공격자로부터 정보의 파괴, 변조, 유출으로부터 보호
- 3대 목표 이외 6대 목표라고 하면 추가되는 목표
  - 책임추적성
  - 인증성
  - 신뢰성

#### 6대 목표

1. 기밀성
   - 정보의 소유자가 원하는 대로 정보의 비밀이 유지되어야 한다는 원칙
   - 정보는 소유자의 인가를 받은 사람만이 접근가능해야하며 인가되지 않은 정보의 공개는 반드시 금지
   - 기밀 자료는 기밀성이 노출되지 않도록 반드시 인가된 자에 의해서만 접근할 수 있어야
   - 기밀성 보장 매커니즘: 접근 통제(물리적, OS, 네트워크), 암호/인증 등
1. 무결성
   비인가자에 의한 정보의 변경, 삭제, 생성 등으로부터 보호되어 정보의 정확성, 완전성이 보장되어야 한다는 원칙
1. 가용성
   정보시스템은 적절한 방법으로 작동하여야 하며, 정당한 방법으로 권한이 부여된 사용자에게 정보서비스를 거부하여서는 안된다는 원칙
1. 책임추적성
   - 각 개체의 행위를 유일하게 추적할 수 있음을 보장하는 것.
   - 정보나 정보시스템의 사용에 대해서 누가 언제 어떤 목적으로 어떤 방법을 통하여 정보 자산을 사용했는지 추적
1. 인증성
   어떤 주체나 객체가 틀림 없음을 보장할 수 있는 것이고 정보시스템 상에서 이루어지는 활동이 정상적이고 합법적으로 이루어진 것을 보장
1. 신뢰성
   의도된 행위에 대한 결과의 일관성을 유지하는 것으로 정보나 정보시스템을 사용함에 있어서 일관되계 오류 발생 없이 계획한 활동을 수행하여 결과를 얻을 수 있도록 하는 환경 유지

#### 정보보호의 특성, 중요성

가치있는 자산을 손실, 오용, 공개 또는 손상으로부터 보호하는 일

#### 보안취약점 및 위협요소

HW 또는 SW의 결함이나 체계 설계상의 허점으로 인해 사용자의 허용된 권한 이상의 동작이나 허용된 범위 이상의 정보 열람을 가능하게 하는 약점

###### 구분

- 물리적 (물리, 자연, 환경)
- 기술적 (HW, SW, 매체, 전자파, 통신)
- 관리적 (인적)

#### 보안 위협

자산의 손실을 초래할 수 있는 원치 않는 사건의 잠재적 원인이나 행위자

###### 분류

- 자연
- 인간의 의도적
- 인간의 비의도적

#### 위험

특정 위협이 취약점을 통해 자산을 공격해 손실을 초래할 수 있는 잠재력

#### 정보보호 대책

위협에 대응하여 정보자산을 보호하기 위한 관리적, 물리적, 기술적 대책

## 사이버 공격 유형

- 해킹: 정당한 권한 없이 정보통신시트템에 침입
- DDoS: 악성코드에 감염된 좀비 PC이용, 대량의 유해 트래픽 전송
- Homepage Defacement: 홈페이지 변조, 이미지 실추 목적
- 피싱: 위장된 홈페이지에 정보 입력하도록 (보이스피싱, 메신저 피싱, 스미싱)
- 스팸: 수신자 의사에 반하여 전송되는 광고성 정보

# 3주차

## 악성코드

악성 행위를 위한 SW

#### 종류와 특징

| 구분        | 내용                         | 자기복제 | 독립 프로그램 |
| ----------- | ---------------------------- | -------- | ------------- |
| 바이러스    | 프로그램을 통한 감염 및 실행 | O        | X             |
| 웜          | 네트워크를 통한 감염 및 실행 | O        | O             |
| 트로이 목마 | 정보 유출                    | X        | X             |
| 애드웨어    | 자동 광고물 표시             | X        | X             |

#### 이 외

- 스파이웨어: 컴퓨터, 프로그램 정보 수집하고 외부에 전송, 개인정보도 유출 가능
- 웜 바이러스: 웜 + 바이러스, 네트워크 자동 전파되며 다른 프로그램, 파일들도 감염
- 봇: 트로이 목마 + 웜, 다수의 PC 탈취, 네트워크 공격 (DDoS 사용)
- 하이재커: 의도치 않는 다른 사이트 이동
- 논리 폭탄: 특정 조건 만족 시 실행, 파악 어려움

## 바이러스

- 최초: 1971년 크리퍼 바이러스 제작
- 현재의 개념: 1986년 브레인 바이러스

#### 종류

- 부트
- 파일

## 웜

최초: 모리스 웜

#### 종류

- 러브레터
- 님다: 메일 첨부파일
- 슬래머: MS SQL Server전파, DoS
- 블래스터: OS

## 악성코드 분석

- 정적: 디스어셈블, 리버싱 - 소스 역 추출
  - 회피 방안: 패킹, 난독화)
  - 선수 지식: OS, 프밍 언어, 프밍, 분석 도구, 프로세스 모니터링 도구
- 동적: 어떤 행위 하는지 직접 판단 (VMWare 등 가상 머신에서 주로 함)
  - 프로세스 확인 / 시작 프로그램 확인 / 파일과 레지스트리 변경 내용 확인 / 파일, 레지스트리, 네트워크 활동 확인

## 사회공학 보안공격

사람 속이는 것

#### 종류

- 쓰레기통 뒤지기
- 어깨너머 훔쳐보기
- 직접 접근
- 도청
- 파밍
- 피싱
- 스미싱
- 랜섬웨어

## 접근 통제

- 자원이 어떻게 접근되는지를 제어하여 인가되지 않는 수정이나 노출로부터 보호하는 것
- 주체와 객체 사이의 흐름

#### 필요성

- 허가되지 않는 접근에 대응하기 위한 첫 번째 방어 수단
- 기밀성, 무결성, 가용성 보호 역할 수행

#### 과정

- 식별: ID
- 인증: PW
- 인가: 접근 권한
- 책임추적성: 로그

#### 인증 유형

- 지식: PW
- 소유: 토큰
- 존재: 생체
- 행위: 서명

#### 강한 인증

인증 방법 2 가지 이상(이중(2), 다중(3+))

#### 모델

- 강제적: 규칙 기반
  - 데이터를 분류, 레이블을 붙이고, 레이블 별 정책
  - 단점: 성능 좋지 않고, 구현 어렵다. 동적 조직에서 채택 힘들다.
  - 모델
    - 벨 라파툴라: 높은 보안수준에서 낮은 수준으로 정보 흐르는 것 방지
    - 비바: 데이터 변형 방지만 해결 (무결성)
- 임의적: 신분 기반
  - 객체에 대해서 접근 권한이 있는지
  - 단점: 중앙 집중적 관리 어려워서 엄격한 접근 제어는 힘들다
- 비임의적: 역할 기반
  - 최소 권한만을 허용하고 직무를 분리하여 특권 X
- 그 외
  - 클락 윌슨
    - 잘 구성된 트랜잭션
    - 직무 분리
    - 사용자의 응용 프로그램을 통한 데이터 접근
  - 만리장성
    - 한 회사에 최근 일을 한 적 있는 파트너는 동일한 영역에 있는 다른 회사 접근 불가라는 개념

#### 기본 원칙

- 직무 분리
- 최소 권한

# 4주차

## 암호

비밀 부호, 약속 기호

## 암호화 과정

- 암호: 다른 사람이 해석할 수 없게 하는 방법
- 평문: 암호화 전 메시지
- 암호문: 암호화 후 메시지
- 암호화(과정): 평문을 암호문으로 바꾸는 것
- 암호화 알고리즘: 평문을 어떻게 암호문으로 변경할지 방법
- 암호화 키: 암호문 강제적 해독을 막는 것.

## 복호화 과정

복호화: 암호문을 복호화 키를 통해 평문으로 바꾸는 것

#### 키와 상호관계

- 대칭: 암호화 키 = 복호화 키
- 비대칭: 다름

## 암호 역사

#### 고전 암호학

###### 스키테일

메시지에 있는 문자 위치 바꾸는 것 (키 = 나무막대 굵기)

###### 시저

- 알파벳 단일 치환 알고리즘
- 전사 공격 취약

#### 단일치환

###### 모노 알파베틱

알파벳 26글자를 각각 다른 알파벳으로 대응
암호화 키: 치환표

#### 다중 치환

- 한 글자가 암호화 키와의 매핑에 따라 여러 글자로 대체되어 암호화
- 빈도분석법에 강함
- 플레이페어, 에니그마로 발전
- 현대는 해독 쉬움

#### 대칭 암호화

- DES
  - 초기 치환
  - 16번 라운드
  - 최종 치환
- 트리플 DES
  - DES 3번 (암호화: 암, 복, 암 / 복호화: 복, 암, 복)
- AES
  - NIST 1997년 공모
  - 128 비트
  - 키 크기 3가지
  - 10번 라운드
  - 각 라운드 (대치, 치환, 혼합, 애드라운드키 연산)
- 그 외
  - SEED (국산 128)
  - ARIA (국산 128)
  - IDEA (유럽)
  - RC5 (미국)
- 블록 암호모드
  - 개념: 하나의 평문을 블록 단위로 나눠서 암호화 또는 복호화 (300비트 평문 AES 암호화, 블록 개수 3개, 3번 째 블록 저장 44비트, 나머지 패딩)
  - 종류
    - ECB: 그대로 암호문 블록, 중간 블록 바꿔치기 가능한 단점
    - CBC: 암호문 블록을 체인처럼 연결, 계산 복잡한 단점

#### 비대칭 암호화

- 개요: 대칭은 키 배포 문제가 관건
- 종류
  - 디피-헬만
    - 소수를 이용한 나머지 연산
    - 통신 통해 미리 배포되지 않은 새로운 비밀키 s를 공유하는 것이 목표
  - RSA
    - 실질적 산업 표준
    - 공개키(외부 공개)와 개인키
- 방식
  - 공개키로 암호화 개인키로 복호화 (기밀성 보장) - 공개기
  - 개인키로 암호화 공개키로 복호화 (부인 방지 보장) - 개공부

# 5주차. 해시

## 해시

- 메시지를 입력하여 길이가 정해진 짧은 값 변환 혹은 압축
- 무결성 확인 목적
- 입력 길이 상관 없이 고정된 길이 값 (압축)

#### 특징

- 일방향성 (역으로 알아내기 불가)
- 충돌회피 (같은 해시 값 없다)
- 효율성 (시간 자원 적다)

#### 용어

- 해시 함수 (메시지 다이제스트 함수)
- 메시지 (프리이미지)
- 해시 결과값 (메시지 다이제스트)
- 무결성 (완전성, 보전성)

#### 대표 종류

- MD: 128비트, MD5 보안 취약점 있어서 사용 X
- SHA: 보안성 더 높고 현재는 SHA-2 권장

#### 목적과 한계

- 목적: 무결성 확인
- 한계: 누가 보냈는지 모름

## 메시지 인증 코드

- 메시지가 올바른 송신자로부터 왔다는 것 확인
- 추가적인 키를 이용 MAC 함수 통해 계산된 값
- 해시와 공통: 길이 정해짐
- 차이: 추가적인 키가 필요
- MAC이 인증 역할: 송수신자 키를 공유해야

#### 예시

- SWIFT
- IPsec
- SSL/TLS

#### 실현방법

HMAC: 해시 함수를 이용하여 메시지 인증 코드 구현하는 방법, SHA256 사용 가능

#### 제약 사항

- 키 배송 문제
- 제 3자 증명 불가
- 부인 방지 불가 (같은 키 공유 때문)

#### 재전송 공격 및 대응 대안

- 기존 정상적 MAC 값 이용 같은 메시지 반복 공격
- 대안
  - 시퀀스 번호: 마지막 번호 기록해두어야
  - 타임스탬프: 송수신자 시간 맞아야
  - 비표: 통신 프로토콜 자체가 달라져야

## 전자서명

- 서류에 대한 인증 및 부인방지
- 원본메시지에 대한 해시 값을 서명자의 개인키로 암호화

#### 공개키 암호와 전자 서명

- 암호화는 공개키로 암호화, 전자서명은 개인키로 암호화 - 암공전개

## 공개키 기반 구조

- 전자서명 약점: 공개키가 정말로 송신자의 공개키인지 증명 필요
- 공개키 인증서: 신뢰할 수 있는 인증기관 통해 안전한 공개키 제공

# 6주차. 시스템 보안

## 시스템

- 시스템: 보안 공격 대상 단위, 대상
- 정보 시스템: 네트워크, 어플리케이션 계층 구성되어 상호작용 통해 정보시스템 구축
- 시스템 보안
  - OS, 응프, 서버 취약점 이용한 공격 방지
  - 3계층 보안 (시스템, 네트웤, 어플)
  - 계정/암호, 서비스, 패치, 로그 관리 필요

# 7주차. 어플리케이션 보안

## 웹

- 하이퍼텍스트 문서들이 인터넷을 통해 연결된 시스템
- 팀 버너스 리

#### 구성요소

- 프로토콜: HTTP
- 콘텐트: 하이퍼텍스트 문서들
- 주소 체계: URL

## HTTP

한 쪽 클라이언트, 한 쪽 서버

#### 요청 메시지

메U프헤 (POST: 메U프헤바)

#### 응답 메시지

프상설헤바

#### 특징

- 비연결지향
- 새로운 요청 마다 새로운 접속
- 1.1 버전: Keep Alive로 얼마동안 접속 열어둘지 설정 가능
- 쿠키: 클라이언트에 저장되는 키와 값이 있는 데이터
- 세션: 서버와 일정시간 같은 클라이언트에서 오는 요청을 하나의 그룹으로 보고 세션으로 식별

## URI

스인호포경파식

## 웹 취약점 및 보안 대책

OWASP (비영리 국제 단체, 10대 보안 취약점 2004년 부터 3년마다 발표)

#### 취약점

- SQL 인젝션 (바인딩, 특문 검증)
- 경로 조작 (특문 검증)
- 위험한 형식 파일 (허용된 확장자만, 임의의 문자열로 변경, 디렉토리 전혀 다른 곳, 실행 속성 제거)
- 크로스사이트 스크립트 (입력값 특문 검증)
- 적절한 인증 없는 중요 기능 허용 (인증 점검 로직)
- 부적절한 인가 (인가 검증 로직)
- 중요 정보 평문 저장 / 전송 취약한 암호화 알고리즘 사용 (반드시 암호화)
- 오류 메시지 부적절 노출

## 웹 서버 관리

- 최소 권한
- 디렉토리 검색 막기 (index)
- 불필요 파일 제거 (OS 알려주지 말기)
- 파일 업로드 및 다운로드 최대 크기 설정
- IIS WebDAV 비활성화

## 로그 관리

- IIS: W3C
- 아파치: httpd.conf
