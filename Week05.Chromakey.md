### Chromakey

> 촬영 시 유의사항

 1. Chromakey란 합성할 피사체를 단색 배경으로 촬영한 다음 그 화면에서 배경색을 제거하거나 투명하게 만들어 피사체만 남게 되는 원리를 이용한다.
 2. 크로마키 촬영은 라이팅이 가장 중요하다. 
 3. 조명을 인물에게만 주었을 경우 배경에 그림자가 만들어지기 때문에 key를 빼는 작업에서 힘들다.
 4. 그래서 조명을 배경 background lighting을 하는 것이 중요하다.
 5. 이럴 경우 인물이 어두워 보일 수 있지만 배경에 그림자가 만들어지지 않는 선에서 조명을 치는 것이 중요하다.
 
 >아래 사진들은 이번 학기 초 촬영한 굿덴이라는 청바지 브랜드 광고 촬영영상이다. (영상, 사진 공유 동의받았습니다.)
 ![chromakey_plate](https://user-images.githubusercontent.com/90584191/146668696-25a9269a-5dc5-4329-8b5f-44f5b6a1ecad.JPG)
 ![chromakey_plate02](https://user-images.githubusercontent.com/90584191/146668723-6e776615-6a2f-45c3-b765-8c8ef63bfb3d.JPG)

>Key light node

* Keylight node를 사용 할 때에는 색을 한번에 뺀다는 생각을 하면 안된다.

* 한번 뺐을 때 피사체의 외곽선이 사라지거나 피사의 외곽선보다 알파가 더 살아있게 된다.


* 그래서 Soft key 와 Hard Key 또는 Soft matte, hard matte로 구분하여 배경색이 확실하게 빠질 때까지 node의 갯수를 늘려서 사용한다.

>Soft key

![chromakey_softkey](https://user-images.githubusercontent.com/90584191/146668850-06a003a0-83f4-4b95-a93a-3bc6322ea113.JPG)
![chromakey_softkey_Alpha](https://user-images.githubusercontent.com/90584191/146668853-f253295e-86b3-4046-81aa-3508a5de5ef7.JPG)

>Hard Key

![chromakey_hardkey](https://user-images.githubusercontent.com/90584191/146668903-8da6b92b-191c-4be7-8f36-3661b090da67.JPG)
![chromakey_hardkey_Alpha](https://user-images.githubusercontent.com/90584191/146668904-7d935129-0ead-4fea-a867-0ca6a8ca6f13.JPG)

## * Soft key와 hard key. 2개의 keylight으로 색이 다 빠졌다고 가정해보자.


## * 이후에 ChannelMerge Node, Key Mix를 통해 두개의 Keylight을 합쳐주고 Copy(alpha to alpha)를 통해 배경색의 alpha를 빼준다.

## > DespillMadness

 정말 촬영을 잘 해왔다고 하더라도 피사체에는 그린이 묻어남을 수 밖에 없다. 그것을 despillmadness node를 통해 제거한다.

# > Grade node

* photoshop도 잘 다루지 못하고 합성 툴을 Nuke로 처음 배워서 그런지 Grade node 는 신세계였다. 색채의 마술사가 된 기분.

* 눈에 잘 보이게 background를 constatnt node를 사용해 단색배경으로 했다.

 일반적인 매
 
![Grade01](https://user-images.githubusercontent.com/90584191/146669315-22be9bcc-0af3-4d6c-9c2e-8fd00ecd80f5.JPG)

Grade node 이후의 매

![grade02](https://user-images.githubusercontent.com/90584191/146669318-22d2baa7-3e11-47ca-8ec7-e45a8b7dea73.JPG)

Grade node를 사용해 현실에 없는 매의 색을 내보았다. 

![grade03](https://user-images.githubusercontent.com/90584191/146669319-b68d127e-661e-489c-8a3e-bd5b4b63aa96.JPG)


 
 
 

