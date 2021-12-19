## WEEK 03
>GAMMA
* 감마는 플레이에 입력되는 신호의 밝기와 화면상에 나타나는 영상의 휘도 간 상관 관계를 결정하는 수치이다.
(https://news.samsungdisplay.com/1869/) ![감마](https://news.samsungdisplay.com/wp-content/uploads/2017/05/2-26.jpg)
* ray부터 255 Gray까지 단계별로 한 칸씩 각각의 밝기를 지정하고, Gray가 올라갈수록 해당되는 Gray의 휘도가 점점 높아지게 설정을 한다. 만약, 감마값이 1이라면 Gray Level에 따른 휘도 값이 정비례하게 나타나게 된다. 
* 하지만, 인간의 눈은 어두운 곳의 차이는 잘 구분하지만 밝은 곳의 차이는 잘 구분하지 못하기 때문에 감마값을 1로 정비례하게 설정을 해 놓는다면 높은 Gray로 갈수록 밝은 색을 잘 구분하지 못하게 된다.
* 이를 보완하기 위해 인간의 눈에 최적화시킨 감마값을 맞추는 것이 중요하다. 그 값이 NTSC(National Television System Committee) 표준 감마값인 **2.2**이다.
>Linear-Workflow
* 모든 그래픽 작업이 선형 색 공간(Linear Color Space)에서 이루어지는 방식을 말합니다.
* 사람의 눈은 베버의 법칙 때문에 밝은 색보다 어두운 색에 훨씬 민감합니다. 베버의 법칙이란 ‘감각기는 약한 자극이 있는 상황에선 자극의 변화가 적어도 자극을 느낄 수 있으나 강한 자극이 있는 상황에선 자극의 변화가 커야 자극을 느낄 수 있는 법칙'입니다. 즉 어두운 환경에선 조금의 빛만 주어져도 감지할 수 있지만, 밝은 환경에선 조금의 빛은 느낄 수가 없다는 것입니다. [https://www.scienceall.com/%EB%B2%A0%EB%B2%84-%ED%8E%98%ED%9D%90%EB%84%88%EC%9D%98-%EB%B2%95%EC%B9%99weber-fechners-law/]
* !!!!!**모든 이미지 파일들이 감마 보정이 된 채 저장되지는 않습니다. png, gif, jpeg 따위의 이미지 파일들은 감마 보정으로 원래보다 밝게 저장되지만, raw, exr 등과 같은 이미지 파일들은 감마 보정이 없습니다. 따라서 이들을 모니터에서 보면 다소 어둡게 나타나는 것입니다.**
* ![리니어감마](https://docs.unity3d.com/uploads/Main/LinearRendering-LightingSphereLinearGamma.png)
>ACES
* ![aces](https://www.oscars.org/sites/oscars/files/styles/hero_image_wide_default/public/aces_main3.png?itok=inY3Kf2j)
* ACES(Academy Color Encoding System)는 영화 또는 TV 프로덕션의 수명 주기 동안 색상을 관리하기 위한 업계 표준이다.(https://www.oscars.org/science-technology/sci-tech-projects/aces)
* ACES는 16bit, 32bit, 25stop 이상의 규격을 가지고 있어 현존하는 모든 카메라의 다이내믹 레인지와 컬러 영역을 커버할 수 있다.(http://journal.kobeta.com/%EC%B0%B8%EA%B4%80%EA%B8%B0-aces-%EC%8B%9C%EC%8A%A4%ED%85%9C/)
* ACES의 이점
 1. 표준화된 보기 변환 및 장비 보정 방법을 통해 온셋 모양 관리와 다운스트림 색상 보정 간의 불확실성 제거
 2. 포스트 프로덕션 및 마스터링 전반에 걸쳐 사용하기 위해 세트에서 캡처한 전체 범위의 하이라이트, 그림자 및 색상 보존
 3. 다른 카메라의 이미지 매칭 단순화
 4. 대체 결과물을 생성할 때 소스 자료의 용도를 변경할 수 있는 수단 제공
> straight & premutiplication
  * ![straight alpha](https://t1.daumcdn.net/cfile/tistory/9975123B5C0FD14335) 
  * "non-premultiplied alpha"는 "straight alpha" 또는 "unassociated alpha"라고도 부르며, 우리가 가장 익히, 편하게, 친숙하게 알고 쓰는 알파 형식입니다.
  * ![premultiplied alpha](https://t1.daumcdn.net/cfile/tistory/99C8A5495C0FD14314)
  * premultiplied alpha"는 "associated alpha"라고도 부르며, 이미지의 필터링과 혼합에 적합한 표현 방식입니다.
  * premultiplied alpha 방식의 RGBA 인코딩은, 그 이름이 암시하듯이 알파 값을 RGB에 미리 곱해 둡니다.
  * RGB에 (불)투명도를 미리 곱해 두면, 알파 값 없이 RGB만 가지고도 투명도가 적용된 색상을 얻을 수 있을 뿐만 아니라, 그래픽 처리시에 필요한 연산이 줄어드는 장점이 있죠.
  * 다시 말해 premultiplied alpha 방식의 RGBA에서 RGB의 값은 그 자체만으로도 색상과 더불어 이미 투명도를 반영하고 있으며, 알파 값은 복잡한 그래픽 처리를 위해서 덤으로 딸려 들어오는 것에 불과    합니다.
그리고 이 방식의 또 한 가지 특징은 RGB 각각의 값이 덤으로 얹어 주는 알파의 값보다 항상 작거나 같다는 점입니다.
