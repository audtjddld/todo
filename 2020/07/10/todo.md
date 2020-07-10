# 알아볼 것


## 디비 파티셔닝
 - 기존 데이터 마이그레이션 할 때, 파티션 형태로 나눠서 적용할지에 대한 부분이 있었다. 사실 개념상으로만 알고 있기 때문에 자세히 알아보자.

## gRPC
 - [프로덕션 환경에서 사용하는 golnag과 gRPC](https://blog.banksalad.com/tech/production-ready-grpc-in-golang/?gclid=EAIaIQobChMIvJ2BxP3B6gIVzGkqCh2ZMgffEAAYASAAEgIWvPD_BwE) 
 golang은 됬고, gRPC 알아보자.


## Redis 원자적 계산 방법
 - 재고 차감 여부를 계산 하는 방법으로 Redis를 이용한 계산을 하는 것을 생각했는데, 방향과 맞지 않는 것으로 판단되었다.
  - 추가적으로 알아본 봐 dbms의 locking 방법을 좀더 면밀하게 적용해서 처리 하는 것 같다.
   - 내부큐 사용은 요청량이 많을 때 애플리케이션 자체에 부담이 생길 수 있음으로, 왠만하면 외부 자원을 끌어다 쓰는 것이 좋아보이는데, 응답 요청 방식에서 어떻게 해야 자연스럽게 줄지는 의문이다.
