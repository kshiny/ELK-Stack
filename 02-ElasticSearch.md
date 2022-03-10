# ElasticSearch

### 왜 ElasticSearch인가?

* Near Realtime(NRT) : 데이터 색인(Indexing) 후 약 1초 후부터 검색 결과에 반영된다.
  ![image](https://user-images.githubusercontent.com/77952321/157584498-bb9f89eb-037f-4d7e-a5f0-2e00a5c081b1.png)  
  
* 모든 Field에 대해 Indexing 처리하므로 검색 처리 시간이 짧다.
  ![image](https://user-images.githubusercontent.com/77952321/157584574-bde9b99c-5003-4cff-9bd8-b5ddbd81ae5e.png)
  
* 운영 중인 elasticsearch cluster에 간단한 설정을 통해 elasticsearch node 추가 가능하다.
  ![image](https://user-images.githubusercontent.com/77952321/157584680-d13e1dc5-fe88-4f4e-8f38-1cefc9fc64f7.png)
  
* Index(≒데이터)를 shards(≒조각)로 세분화하여 여러 operations 성능 향상된다.
  ![image](https://user-images.githubusercontent.com/77952321/157584934-554958e6-dfe8-48ba-8755-60fcd091816e.png)

* (Replica Shards를 설정을 통해) 특정 Node (≒서버)가 다운되어도 데이터 유실 없이 운영할 수 있다.
  ![image](https://user-images.githubusercontent.com/77952321/157585083-a73a6999-5b0f-46d9-806f-d2ffa9246c16.png)

* 아래의 비교는 어디까지나 이해를 돕기 위할 목적일 뿐 정확히 일치하지 않는다.
  ![image](https://user-images.githubusercontent.com/77952321/157595020-dc4fd670-ab89-48a8-857c-abec252de175.png) 
    
  ![image](https://user-images.githubusercontent.com/77952321/157595140-2b10ed55-0c48-4c55-866b-7533838cdf41.png)
  ![image](https://user-images.githubusercontent.com/77952321/157595272-8d81126e-1220-4b00-b202-31d38360c4ae.png)
  ![image](https://user-images.githubusercontent.com/77952321/157595219-380c3f9f-453e-49f8-b367-0a5f94f2b361.png)
  ![image](https://user-images.githubusercontent.com/77952321/157595327-3853ba8c-e887-49f4-b24c-8dec34d22501.png)
  ![image](https://user-images.githubusercontent.com/77952321/157595376-efa5b107-471f-4852-a141-f94945835859.png)
