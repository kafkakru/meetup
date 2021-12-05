#### About 1st Meetup
---
* Date : 2018-09-08 (Saturday)
* Time : 14:00 ~ 18:00 Korea Standard Time
* Venue : Microsoft Korea
* Attendees : 30+
* Speakers
    * 이기화 : [Data Pipeline @KakaoStory]
    * 강대명 : [별쓸모없는이야기 Spark, 그리고 Kafka timestamp offset]
    * 이동진 : [Testing Kafka Streams Applications]
    * 문규원 : [Kafka 활용 비동기 시스템 구성]
    * 류지형 : [Kafka 사용 사례]
* Questions
  &nbsp;

  ```
  - 람다 아키텍처와 카파 아키텍처의 장단점 좀 알려주실 수 있을까요?
  - 질문 타임 인덱스는 프로듀서가 넣어주는게 맞나요? 로그스태시가 타임 인덱스를 넣어주지 않는다고 하는데, 추가하려면 어떻게 하는지 간략하게 설명좀 부탁합니다.
  - 인덱스 파일이 기본으로 10MB로 만들어지는데, 세그먼트 롤링되면 10MB보다 더 작아지던데, 기본으로 10MB로 잡는 이유를 혹시 알 수 있을까요?
  - 설명해주신 테스트 전략은 Spark streaming개발시에도 사용 가능한가요?
  - 다른 stream처리 오픈소스와 차별화되는 kafka streams 만의 장점이 있나요?
  - 카프카와 래빗앰큐의 쓰루풋이 어느정도 차이 나는 지 알 수 있을까요? 그리고 래빗앰큐는 클러스터링을 해도 복제라 쓰루풋이 안 올라간다고 하셨는데 그럼 높은 쓰루풋이 요구 되고 스케일링이 필요한 상황이면 래빗앰큐를 사용하지 않고 카프카를 써야하는 것이 맞나요?
  - 큐에서 메시지를 꺼내서 처리하다가 실패하는 경우가 구체적으로 어떤 경우가 있나요?
  - logstash에서 직접 file input 사용시 sincedb에서 inode 문제를 지적해주셨는데요. 저는 filebeat-> kafka -> logstash -> elasticsearch 와 같이 사용하는데 이런 경우 위의 문제를 회피한다고 봐도 될까요?
  - 선호하시는 retry interval값과 횟수가 있으신가요?
  - 컨슈머 장비가 여러대이고 장비 마다 순차배포할때라면 계속 컨슈머 리밸런싱이 일어날텐데 어떤식으로 처리하고 계신지 알 수 있을까요?
  - 모든 하둡에코의 모든 로그를 수집하나요? 아님 에러로그만 수집을하나요? 수집한 로그를 검색할 때는 어떤 채널을 이용하나요?
  - telegraf를 통해 모니터링을 하셨는데 성능문제나 서비스에 문제를 준적은 없었나요?
  - 모니터링 하는 data lake의 규모는 어떻게 되나요?
  ```
* Reference
    * [kafka-streams-example](https://github.com/dongjinleekr/kafka-streams-example)
    * [logstash-output-kafka specify timestamp](https://github.com/logstash-plugins/logstash-output-kafka/pull/125)
