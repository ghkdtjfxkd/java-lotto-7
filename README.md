# java-lotto-precourse

# 🏃 학습 목표

---
- [ ] 관련 함수를 묶어 클래스 만들기
- [ ] 클래스와 함수에 대한 단위 테스트를 통해 의도한 대로 작동하는 영역 확보
- [ ] 2주차 공통 피드백 반영
    - [ ] 기능 목록 작성 시 메서드 설계나 구현 같이 상세한 내용 포함하지 말 것
    - [ ] 정상적인 상황 뿐만 아니라 예외 사항도 함께 정리하기
    - [ ] 기능 목록 업데이트 하기

#  🛠️ 기능 목록

## 🕹️ 진행

---
### ✏️ 입력
- [x] 입력을 받고 반환한다.
- [x] 로또 구입 금액을 입력 받는다.
- [x] 로또 당첨 번호를 입력 받는다.
- [x] 보너스 번호를 입력 받는다.
- [ ] 잘못된 값을 입력하면 에러를 발생
    - [ ] 에러 메시지 출력
    - [ ] 입력 다시 받기

### 👀 검증
- [x] 공용 검증
- [x] 로또 구입 금액 검증
- [x] 로또 당첨 번호 검증
- [x] 보너스 번호 검증

### ♻️ 입력 값 형 변환
- [x] 문자열을 숫자로 변환한다.
- [x] 문자열을 문자열 리스트로 변환한다.
- [x] 문자열 리스트를 숫자 리스트로 변환한다.

### 🎛 입력 값 분배
- [ ] 발행 로또 수량 설정
- [ ] 로또 당첨 검증용 번호 설정
- [ ] 보너스 번호 검증용 번호 설정

### 🎉 로또 1 게임 (자동)
- [x] 무작위 6개의 숫자 생성한다.
- [x] 6개의 숫자 오름차순으로 정렬한다.
- [x] 무작위 6개의 번호 반환한다.

### ⚙️ 로또 기계 (로또 게임 생성)
- [ ] 로또 수량을 기반으로 로또 용지를 생성한다.
    - [x] 로또 생성
    - [ ] 로또 저장
- [ ] 로또 용지(로또 게임 모음) 반환한다.

### 🎫 로또 티켓
- [x] 로또 게임 저장
- [x] 로또 게임 반환
- [x] 게임 횟수 관련 정보 반환

### 🛖 로또 가게
- [x] 돈을 받고 로또 게임 횟수를 결정한다.
- [x] 로또 게임 횟수만큼 로또 게임이 담긴 로또 기계를 반환한다.

### 🏦 은행(지급사)
- [ ] 로또 용지를 입력 받아 검증한다.
- [ ] 당첨금을 지급한다.

### 🔍 검증 기계
- [ ] 정해진 당첨 번호와 입력된 로또가 가진 동일한 번호의 갯수를 센다.
- [ ] 동일한 갯수를 반환한다.
- [ ] 등수를 반환한다.
- [ ] 당첨급 보고서를 반환한다.

### 📈 당첨금 보고서
- [ ] 일치하는 번호의 갯수를 반환한다.
- [ ] 일치하는 번호의 유형을 반환한다.
- [ ] 수익률을 반환한다.

### 🖨️ 출력
- [ ] 일치하는 유형을 출력한다.
- [ ] 일치하는 번호 유형에 따른 당첨금을 출력한다.
- [ ] 일치하는 유형의 수를 출력한다.
- [ ] 수익률을 출력한다.

## 🚧 예외 상황

---

### ✏️ 입력
#### 🧩 공통
- [ ] 빈 값 입력
- [ ] 공백 문자 입력
- [ ] 공백 문자가 포함된 입력

#### 🧩 구매 금액
- [ ] 숫자를 제외한 문자가 섞인 입력
- [ ] 오버 플로우를 발생시키는 값 입력
- [ ] 0 입력
- [ ] 1000 으로 나누어 떨어지지 않는 값 입력

#### 🧩 로또 공(당첨 번호, 보너스 번호)
- [ ] 숫자와 구분자를 제외한 문자가 섞인 입력
- [ ] 중복되는 숫자가 존재하는 입력
- [ ] 오버플로우를 발생시키는 값
- [ ] 지정한 로또 공 숫자 범위를 벗어나는 숫자가 섞인 입력

