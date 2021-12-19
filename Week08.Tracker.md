## Planar Tracker
 * 간판을 바꾼다는 예시
   * 로토로 간판의 사각을 잡아준다. 각을 잡을 때 감마값을 줄인다던지 색을 조절하면서 확실하게 포인트를 잡는다.
    
   * 이후에 Roto node 안에 있는 cornerpin2d를 생성하여 달아준다.
    
   * 대체할 간판의 이미지를 shuffle, reformat, edge blur, grade node를 사용하여 주변 환경과 유사하게 만든다.
    
   * 이후 merge를 통해 간판이미지를 교체한 것을 확인 할 수 있다.



## Camera Tracker

* camera tracker가 nuke를 상업표준으로 만들어준 1등공신 중 하나다.

* tab 키를 누르면 3d view를 확인할 수 있다.

* Camera, Scene, Scanlinerender가 있다면 3D secen을 만들 수 잇다.

* camera를 움직이면서 animation을 만들 수도 있다.

* 3D node는 빨간색이다.
* 에러 값을 낮추기 위해 피쳐의 갯수를 많이 만들어서 에러 값을 낮춘다.


 > 움직이는 물체와 배경
 * 움직임이 방해가 되는 경우 Roto를 따로 따서 Mask를 Alpha로 빼준다.
 * 위치 정보를 point cloud로 보여준다. 
 
 
 > 과제
 * photoshop에서 psd파일로 저장하고 누크로 불러오면 photoshop에서 만들었던 이미지를 레이어 그대로 Breakout Layers를 할 수 있다.
 
 - psd 파일을 불러오는 이유. 각각의 레이어들을 3d card node에 연결하고 카메라에서 이미지의 거리를 잡으면 depth를 만들어 낼 수 있다.
 - 여기에 3D object를 넣어 영상의 depth를 느낄 수 있다.
 
 
 > 방법숙달이 생명...

