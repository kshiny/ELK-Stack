## Kibana
### Discover : 데이터 검색 및 필터 등을 이용한 간단한 EDA(탐색적 데이터 분석) 작업
![image](https://user-images.githubusercontent.com/77952321/157610012-4bb407fd-36c2-4637-ab73-99a6fd70b12b.png)

### Visualize : Dashboard에 배치할 Visualization 생성
![image](https://user-images.githubusercontent.com/77952321/157610272-84a9bf9e-d71d-407b-8e58-210f4341676a.png)

### Timelion : Visualization의 하나인 (시계열에 특화된) Timelion 생성
![image](https://user-images.githubusercontent.com/77952321/157610441-6a420561-2b29-45c1-b211-6babf3cb725b.png)

### Dev Tools : Elasticsearch REST API를 위한 UI
![image](https://user-images.githubusercontent.com/77952321/157610550-57452e05-a134-4eb2-9391-8ed08a21a68b.png)

### Management : Kibana 설정 수정
![image](https://user-images.githubusercontent.com/77952321/157610637-a6f75eef-3e4c-4bc2-b050-9b281f25cf97.png)
<br></br>
## Kibana 시각화의 전제 조건
1. 데이터가 Elasticsearch Index에 저장되어 있어야 한다
2. 시각화되고 싶은 데이터가 담긴 Elasticsearch Index (혹은 Pattern)을 Kibana에서 등록해야 한다

## Index Patterns 등록 1단계 - Elasticsearch Index(Patterns) 등록
1. Kibana -> Management -> Index Patterns -> Create Index Pattern
2. 시각화 하고 싶은 Index (Patterns) 입력, 예) Index 이름 : Shopping
3. Next step 클릭

