## ElasticSearch
* ES는 데이터 분산 저장한다. 그리고 테이블에 행과 열의 방식으로 데이터를 저장하는 것이 아니라 JSON으로 직렬화하여 저장한다. 만약 클러스터가 여러개의 ES 노드로 구성되어 있다면 저장된 document들은 클러스터에 분산 저장되어 어떤 노드에서든 접근이 가능하다.  
<br></br>
* Document가 저장되면 index가 되어 1초안에 거의 실시간으로 검색이 가능하다. ES는 Inverted Index라는 자료구조를 사용하여 매우 빠른 Full-Text-Search(FTS)가 가능하다. Inverted Index는 document 안에 존재하는 모든 유니크한 단어들을 정리하여 그 단어가 포함된 document들을 찾아낸다.
* Index는 최적화된 document들의 모음이라고 할 수 있다. 그리고 각각의 document들은 key-value로 구성된 데이터들을 저장하는 field들로 구성된다.  ES는 기본적으로 모든 field들을 인덱싱하며 각각의 인덱싱된 field들은 최적화된 자료구조를 가지고 있다. 텍스트로 구성될 field들은 Inverted Indices 자료구조로 저장되고, 숫자와 위치정보 field들은 BKD 트리 구조로 저장된다. 이렇게 각각의 필드에 맞춤 자료구조를 사용하는 것이 ES가 매우 빠른 이유이다.

![image](https://user-images.githubusercontent.com/77952321/150712688-36339b11-fa29-4892-947c-b58ff0811487.png)

<br></br>
![image](https://user-images.githubusercontent.com/77952321/150712879-4f8dc28a-e977-45e7-b44f-0ee34160a352.png)
* 자료구조를 보면 가장 큰 개념이 index이며, 그 안에 type이 있고, 그 안에 여러개의 같은 document가 있다.  

![image](https://user-images.githubusercontent.com/77952321/150714486-c3e9ea1c-9852-453d-bec5-95489e91b72a.png)
