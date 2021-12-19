## WEEK 04
> MERGE
<img width="468" alt="merge" src="https://user-images.githubusercontent.com/90584191/137580425-b088eef8-f044-4bd7-9356-62dc06e4f6b5.png">

> Roto(scoping)


 1. 로토스코핑('roto'라고도 함)은 애니메이션 및 실사 프로젝트 모두에 대한 그래픽 자산을 생성하는 프레임별로 실사 푸티지를 추적하는 것과 관련된 애니메이션 기술.
 2. Roto node는 베지어 커브만 있다. e 를 눌러 페더 값을 조정할 수 있다.
 3. 로토를 그릴 때에는 곡선이 많은 부분부터 시작을 하여 점을 최소한으로만 사용하는 것이 좋다.
 4. 점을 최소한으로 사용하더라고 곡선이 있는 부분을 확실하게 체크하고 Grade Node를 사용하여 색을 조절한 후에 로토를 따는 것도 방법이다.
 5. 로토를 하면서 느낀점. 이미지 시퀀스에 레퍼런스 이미지를 잘 살펴보고 프레임 하나하나 잘 만져줘야 할 것 같다.
![roto](https://user-images.githubusercontent.com/90584191/146668318-cf1ed94c-6ef8-4fe6-a1be-3666cf65b549.JPG)
![roto2](https://user-images.githubusercontent.com/90584191/146668327-88c0fd4a-58b2-46e8-aae3-852c3682a790.JPG)

> Rotopaint

 1.로토 스코핑, 장비 제거, 가비지 매트 작업에 도움이되는 벡터 기반 노드이다. 
 2.포인트 별 및 글로벌 페더, 모션 블러, 블렌딩 모드 및 개별 또는 계층 적 2D 변환도 가능하다.
 3.Background와 Mask 크게 두 타입으로 나뉜다.  
 
> Merge

 1. Merge node는 블렌딩 연산을 사용하여 두 개의 노드를 결합 할 수 있도록 포함하고, 마스크 블렌딩에서 영역을 마스크에 입력한다.
 2. 가장 기본적이면서 가장 어려운 node인 것 같다. input과 output에 어떤 채널을 달아주느냐에 따라 결과는 아주 다르다.
 3. B파이프가 항상 아래로 내려오게 하는 것이 노드 정리 시에 가장 보고 좋고 편하다.

![merge1](https://user-images.githubusercontent.com/90584191/146668210-dc471dfc-dd98-4c74-ba65-3aa47a74a620.JPG)
