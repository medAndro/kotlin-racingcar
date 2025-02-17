# kotlin-racingcar

### 1. 자동차 이름 및 시도 횟수 초기화

- 사용자로부터 자동차 이름과 시도 횟수를 입력받아 게임을 초기화합니다.
- 자동차 이름은 쉼표(,)로 구분하여 입력받고, 각 자동차 이름은 1자 이상 5자 이하, 중복 없이 구성되어야 합니다.
- 시도 횟수는 양의 정수(자연수)를 입력받습니다.
- 입력 과정에서 유효성 검사에 실패할 경우 예외를 던집니다.
- 입력받은 자동차 이름과 시도 횟수를 기반으로 RacingGame 객체를 생성하고, 게임을 준비합니다.

### 2. 게임 실행 및 결과 저장

- "실행 결과" 문구를 통해 실행 결과를 명확하게 안내합니다.
- 입력받은 시도 횟수만큼 3번의 내용을 반복합니다

### 3. 경주 반복 실행

- 이동 거리는 0에서 9 사이의 정수 난수를 발생시켜, 4 이상일 경우 1만큼 증가시킵니다.
- 각 자동차의 이름과 현재까지의 이동 거리를 출력합니다.
- 각 실행 사이에 빈 라인을 출력하여 결과를 시각적으로 구분합니다.

### 4. 최종 우승자 출력

- 모든 경주가 종료된 후, 가장 멀리 이동한 자동차를 우승자로 결정합니다.
- 우승자가 여러 명일 경우 모두 우승자로 처리합니다.
- "최종 우승자 : " 문구와 함께 우승자 이름(들)을 출력하여 게임 결과를 명확하게 안내합니다.

### 5. 예외 처리

- 다음과 같은 예외 상황에 대해 적절한 예외 처리를 수행합니다.
- 공백을 입력 하였을 경우
- 참가자 수가 1명 미만인 경우
- 자동차 이름이 1자 미만 5자 초과인 경우
- 앞 뒤 공백이 제거된 자동차 이름에 중복이 있는 경우
- 시도 횟수가 1 미만의 양의 정수인 경우
- 시도 횟수를 숫자로 변환할 수 없는 경우
- 예외 발생 시, 사용자에게 적절한 오류 메시지를 출력하고 게임을 종료합니다