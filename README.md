# 키친포스

## 요구 사항

- 메뉴
    - [ ] 메뉴를 추가할 수 있다
    - [ ] 모든 메뉴를 조회할 수 있다
    - [ ] 메뉴 가격은 0원 이상이다
    - [ ] 메뉴의 가격은 메뉴별 메뉴상품 가격의 총합보다 클 수 없다
    - [ ] 메뉴묶음을 가지고 있다
    - [ ] 메뉴는 메뉴상품 목록을 가지고 있다

- 메뉴묶음
    - [ ] 메뉴묶음을 추가할 수 있다
    - [ ] 모든 메뉴묶음을 조회할 수 있다

- 주문
    - [ ] 새로운 주문을 받을 수 있다
    - [ ] 주문은 주문품목명을 한 개 이상 갖고 있어야 한다
    - [ ] 주문의 주문테이블이 비어있으면 안된다
    - [ ] 주문의 주문테이블이 테이블묶음이면 가장 작은 주문테이블번호가 주문테이블이다
    - [ ] 새로운 주문 상태는 요리중이 된다
    - [ ] 모든 주문을 조회할 수 있다
    - [ ] 주문상태를 변경할 수 있다
    - [ ] 동일한 주문상태로 변경할 수 없다
    - [ ] 주문상태는 요리중, 식사중, 완료 상태를 갖는다
    - [ ] 주문상태가 완료면 상태를 바꿀 수 없다 

- 주문품목명
    - [ ] 메뉴번호와 주문번호를 가지고 있다
    - [ ] 주문한 수량을 가지고 있다

- 주문테이블
    - [ ] 주문테이블을 추가할 수 있다
    - [ ] 모든 주문테이블을 조회할 수 있다
    - [ ] 테이블묶음번호를 가지고 있다
    - [ ] 주문테이블이 비어있지 않고 손님이 0명 이상이면 손님 인원을 변경할 수 있다
    - [ ] 빈 주문테이블인지 확인할 수 있다
    - [ ] 테이블묶음에 포함되지 않고 요리중 또는 식사중 상태가 아니면 주문테이블를 비울 수 있다

- 상품
    - [ ] 상품을 추가할 수 있다
    - [ ] 가격은 0원 이상이다
    - [ ] 모든 상품을 조회할 수 있다

- 테이블묶음
    - [ ] 주문테이블 목록을 가지고 있다
    - [ ] 테이블묶음을 추가할 수 있다
    - [ ] 테이블묶음 추가는 주문테이블 2개 이상만 가능하다
    - [ ] 테이블묶음 추가할 때 주문테이블이 비어있지 않고 소속된 테이블묶음이 없어야 한다
    - [ ] 테이블묶음에 속한 모든 주문테이블이 요리중 또는 식사중 상태가 아니면 테이블묶음을 삭제할 수 있다

## 용어 사전

| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 메뉴상품 | MenuProduct | 메뉴, 상품과 수량을 관리하는 용도 |
| 메뉴묶음 | MenuGroup | 여러 메뉴를 하나로 묶는다 |
| 주문품목명 | OrderLineItem | 주문 받은 메뉴와 수량 |
| 주문테이블 | OrderTable | 주문 받은 테이블의 손님 인원과 빈 테이블 여부를 체크할 때 사용 |
| 주문상태 | OrderStatus | 요리중(COOKING), 식사중(MEAL), 완료(COMPLETION) 상태를 갖는다 |
| 주문 | Order | 주문 테이블, 주문 상태, 주문 품목명을 갖는다 |
| 테이블묶음 | TableGroup | 단체 손님 받을 때 사용. 주문테이블 여러 개를 하나로 묶는 용도 |
| 손님 | Guest | 메뉴를 주문한 손님 |
| 상품 | Product | 메뉴를 구성하는 상품명, 가격 표시 |

## 모델링

- 
