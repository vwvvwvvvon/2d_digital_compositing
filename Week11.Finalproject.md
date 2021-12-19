##11Weeks

tracker를 창문에 4point tracking을 시도하였다.

![week11](https://user-images.githubusercontent.com/90584191/146673602-42a50d2a-8ead-4e00-a2a5-0ba5cd5d7325.JPG)

소스가 무거워서 합성에 애먹고 있다.

![week111](https://user-images.githubusercontent.com/90584191/146673604-33ee0ea7-2461-4847-b99f-275f707db68d.JPG)

덩쿨을 달아보았는데 티가 난다.

![week1111](https://user-images.githubusercontent.com/90584191/146673606-8e978916-9e9e-4377-ab9d-a17c28b79137.JPG)

## 피드백

* 2D 트래킹으로는 힘들 수 있다. 레퍼런스 프레임을 잘 찾아서 planar tracking을 쓴다.
* 평면적이기 때문에 크게 문제 없을 것이다. 
* 4point cornerpin으로 옮겨서 사용하면 된다.
* 같은 소스이지만 time offset node를 사용하면 다른 소스인 것 처럼 느껴진다.
* frmae range를 loop로 바꾸어 계속 돌아가게 한다.
* vine들이 색을 주변환경과 맞추어야한다.
* vine이 화질이 좋아서 blur로 맞춘다.
* burnmark shuffle node를 달고 알파를 rgba에 다 넣어주고 premult해주면 된다.
