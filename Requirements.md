## 기능적 요구사항

| 도메인 | 기능명         | 설명                                                                                                                |
|----|-------------|-------------------------------------------------------------------------------------------------------------------|
| 유저 | 포인트 조회      | 유저는 자신이 보유한 포인트를 조회할 수 있습니다                                                                                       |
| 유저 | 포인트 충전      | 유저는 상품 구매를 위한 포인트를 충전할 수 있습니다                                                                                     |
| 유저 | 포인트 사용      | 유저는 포인트를 사용하여 상품을 결제할 수 있습니다                                                                                      |
| 상품 | 상품 조회       | 특정 상품을 조회하여 이름, 가격, 수량을 확인할 수 있습니다                                                                                |
| 상품 | 전체 상품 조회    | 모든 상품을 조회하여 이름, 가격, 수량을 확인할 수 있습니다                                                                                |
| 상품 | 인기 판매 상품 조회 | 현재 일을 기준으로 최근 3일간 가장 많이 판매된 상품 N개를 조회할 수 있습니다                                                                     |
| 주문 | 상품 주문       | 유저는 아직 재고가 남아있는 상품을 주문할 수 있습니다                                                                                    |
| 주문 | 주문 조회       | 유저는 단건의 주문 내용을 조회하여 주문한 상품의 이름, 가격, 주문 수량과 주문 상태를 확인할 수 있습니다 <br/>주문 상태 종류 : [주문취소, 결제 전, 결제완료, 배송전, 배송중, 배송 완료] |
| 주문 | 전체 주문 조회    | 유저는 모든 주문의 내용을 조회하여 주문한 상품의 이름, 가격, 주문 수량과 주문 상태를 확인할 수 있습니다 <br/>주문 상태 종류 : [주문취소, 결제 전, 결제완료, 배송전, 배송중, 배송 완료]  |
| 주문 | 주문 취소       | 유저는 [결제 전, 결제 완료, 배송 전] 상태의 주문을 취소할 수 있습니다                                                                        |
| 결제 | 결제          | 유저는 취소되지 않은 주문을 포인트를 사용하여 결제를 요청할 수 있습니다                                                                          |
| 결제 | 결제 조회       | 유저는 주문의 결제 상태를 조회할 수 있습니다.. <br/>     결제 상태 종류: [결제 전, 결제 완료, 결제 취소]                                      |
| 쿠폰 | 쿠폰 조회       | 유저는 현재 자신이 사용할 수 있는 쿠폰을 조회할 수 있습니다 <br/>쿠폰 상태 종류: [발급됨, 사용됨]                                                      |
| 쿠폰 | 쿠폰 사용       | 유저는 쿠폰을 사용하여 할인된 금액으로 상품을 구매할 수 있습니다                                                                              |
| 쿠폰 | 선착순 쿠폰 발급   | 유저는 선착순으로 제공되는 쿠폰을 발급 받아 등록할 수 있습니다                                                                               |

## 비기능적 요구사항
* 선착순 쿠폰 발급로 인해 특정 시간대에 트래픽이 몰려 짧은 시간에 많은 요청이 들어오더라도 버틸수 있어야한다
