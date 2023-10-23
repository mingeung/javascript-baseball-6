### 1. 어떤 기능들이 필요한가?

1. 컴퓨터는 1에서 9까지 서로 다른 임의의 수 3개를 선택한다.

@woowacourse/mission-utils의 Random 및 Console API를 사용하여 구현해야 한다.
Random 값 추출은 Random.pickNumberInRange()를 활용한다.
사용자의 값을 입력 받고 출력하기 위해서는 Console.readLineAsync, Console.print를 활용한다.

2. 게임 시작 문구 출력 "숫자 야구 게임을 시작합니다."
3. 플레이어로부터 3개의 숫자를 입력받는다. "숫자를 입력해주세요 :"
4. 입력 받은 값에 대해서 결과를 출력한다.

1) 같은 수가 같은 자리에 있으면 1스트라이크
2) 같은 수가 다른 자리에 있으면 1볼
3) 같은 수가 전혀 없으면 낫싱

4. 컴퓨터가 생각한 숫자를 모두 맞추면 게임이 종료된다.
5. 게임을 종류한 후 게임을 다시 시작하거나 완전히 종료할 수 있다.
   "3개의 숫자를 모두 맞히셨습니다! 게임 종료"
   -> 게임이 끝난 경우 재시작/종료를 구분하는 1과 2 중 하나의 수
   "게임을 새로 시작하려면 1, 종료하려면 2를 입력하세요."
6. 사용자가 잘못된 값을 입력한 경우 throw문을 사용해 예외를 발생시킨후 애플리케이션은 종료되어야 한다.

### 어떤 객체들로 이루어져 있는가?

여기서 객체란 특정한 역할을 담당하는 주체 또는 요소를 말한다.

💻컴퓨터
1부터 9까지 중의 숫자 중에 3개의 랜덤한 숫자를 뽑는다.
🙋‍사용자
속성: 숫자 3개
행동: 컴퓨터의 숫자를 예측해서 숫자 3개를 입력한다.

🫥문제 내는 사람
속성: 사용자의 숫자, 컴퓨터의 숫자
행동: 사용자의 숫자와 컴퓨터의 숫자를 비교하고 결과를 제공한다.