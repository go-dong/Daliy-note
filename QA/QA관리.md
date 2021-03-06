# QA는 어떻게 하는게 좋은가?

### 시나리오 작성
1. 사용성이 많은 페이지의 시나리오를 먼저 짜는 것이 좋다.
2. 요구사항을 정리한다.
3. 정상 동작(v1) / 동작 안함(v1) / 예외 상황(v2) 으로 나눠서 정리한다.
4. 동일한 케이스로 간주 되는 것들의 세트를 간추려서 한두개만 테스트 한다.


### 참고
- 코드 커버리지가 70%를 넘지 않아야한다.
  (100%는 테스트할 필요가 없는 부분까지 하게되면 불필요한 시간을 할애하기 때문)
- 코드를 리팩토링 할 때 테스트를 변경하는 일이 적도록 코드 작성 전에 미리 밑작업을 하는게 좋다.
  ex) Cypress 중 data-cy, data-test 등..
- 팀이 크지 않다면 통합 테스트 위주로 작성하는 것이 좋다.


### 테스트 코드의 과정 & 결과 중
1. 실행 속도가 빨라야 한다.
2. 내부 구현이 깨지지 않아야 한다.
3. 버그를 검출 할 수 있어야 한다.(당연하다)
4. 테스트의 결과가 안정적 이여야 한다.(최근 기술 중 Cypress 가 그나마 안정적)
5. 의도가 명확히 드러나야 한다.


### 코드 구분
- it()은 영역별로 나누어 구분한다.
ex)
```cpp
describe('', () => {
  it('search section', () => {
    // search section
  });

  it('list section', () => {
    // list section
  })
})
```
