# 🏎 kotlin-racingcar-precourse
## 📚 기능 목록

### Model
#### RacingCar
- 각 자동차의 이름과 이동 거리를 저장
- [x] 자동차 이름을 저장
- [x] 이동한 거리를 저장(초기값은 0)

### View
#### `InputView`
- 사용자의 입력을 담당
- [x] "경주할 자동차 이름을 입력하세요.(이름은 쉼표(,) 기준으로 구분)" 출력
- [x] 경주할 자동차 이름을 입력
- [x] "시도할 횟수는 몇 회인가요?" 출력
- [x] 시도할 횟수를 입력
#### `OutputView`
- 데이터 출력을 담당
- [x] 실행 결과 문자열 출력
- [x] 최종 우승자 문자열 출력
### Controller
#### `RacingCarController`
- 전체적인 로직을 담당
- [x] 입력한 자동차 이름 개수만큼 RacingCar 객체를 생성
- [ ] 입력한 이름에 대한 검증
- [ ] 시도할 횟수 입력 검증
- [ ] 0~9 사이의 무작위 숫자 생성
- [ ] 생성된 숫자가 4 이상이면 자동차 전진 
- [ ] 차수별 실행 결과 출력
- [ ] 최종 우승자 출력(2명 이상일 경우 쉼표로 구분)
### Constant
#### `PrintMessage`
- 출력할 상수를 담당
- [x] 출력 문자열 선언
#### `ErrorMessage`
- 에러 메시지를 담당
- [ ] 에러 메시지 문자열 선언

### 예외 처리
**자동차 이름 입력**
- [x] 같은 이름이 입력될 경우(예: "pobi,pobi")
- [ ] 빈 문자열일 경우(예: "")
- [ ] 이름의 길이가 5글자 초과할 경우(예: "racingcar")

**시도할 횟수 입력**
- [ ] 숫자가 아닌 문자를 입력할 경우(예: "^")
- [ ] 음수 또는 0을 입력한 경우 (예: "-1", "0")