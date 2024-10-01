


## 텍스트 효과


![bandicam2024-10-0101-53-28-143-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/be00d605-7e29-4078-b55c-f6ab94f7b588)<br/>
![텍스트 효과](https://github.com/user-attachments/assets/06024fd4-fdf6-4c89-93d2-d152363141ce)<br/>

+ linear-gradient() <br/>
  두 개 이상의 색이 직선을 따라 점진적으로 변화하도록 한다. <br/>
  사용 방법은 linear-gradient(방향_또는_각도, 색상_그리고_정지점1, 색상_그리고_정지점2, ... 색상_그리고_정지점n) <br/><br/>


+ background-clip<br/>
  배경 이미지의 위치 기준점을 설정한다. <br/>
  즉, 요소의 배경 (색상이나 이미지)이 어느 부분까지 차지할 지를 설정함.<br/>
  background-clip 기준점은 border, padding, text, 컨텐츠에 설정할 수 있다.<br/>
  text 속성은 베타 버전이기 때문에 접두사 (-webkit)을 표현해주어야 한다.<br/><br/>

+ -webkit-text-fill-color: transparent;<br/>
  배경색이 지정된 요소의 경우 배경색을 없애주어야한다.<br/>
  background의 색상을 없앨 때 none(없애기), transparent(투명)을 사용할 수 있다.<br/><br/>

+ animation-fill-mode <br/>
  애니메이션이 끝난 후의 상태를 설정한다.<br/>
  forwards는 애니메이션의 끝난 후 그 지점에 그대로 있는 상태이다.<br/>

+ white-space  <br/>
  줄바꿈, 공백을 설정한다.<br/>
  white-space: nowrap;은 줄바꿈, 공백을 인식하지 못하며 한 줄로 정렬한다.<br/>

<br/>
<br/>
<br/>




## 마우스 스크롤 애니메이션


![bandicam2024-10-0101-34-59-245-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/2cdfa46c-bf18-4934-a5e4-af8e5b010435)<br>
![마우스 아이콘](https://github.com/user-attachments/assets/c8426033-432a-442e-a61f-598efe173c84)<br>
![마우스 아이콘 1](https://github.com/user-attachments/assets/5185a87b-9459-4339-a767-f25f3c99d6a7)<br>

+ position : fixed를 이용해 위치를 고정시키고 마우스 모양을 만들어주었다.

![마우스 아이콘 2](https://github.com/user-attachments/assets/cccfde54-3e10-4db3-b52d-e34379ac6119)<br>

 :before 가상요소 선택자를 사용하여 'SCROLL' 글자를 넣어주었다.

![마우스 아이콘 3](https://github.com/user-attachments/assets/be4797d1-3abd-40aa-b861-6234434a3779)<br>

마우스 가운데에 볼이 움직이도록 애니메이션을 넣어주었다.<br>
translateY를 이용해서 현재의 위치에서 Y축으로 위 아래로 움직이도록 모션을 만들어주었다.<br>
ease-out을 사용해 애니메이션이 부드럽게 실행되도록 해주었다.<br><br>

+ ease: 천천-빠름-천천<br>
+ ease-in: 보통-빠르게<br>
+ ease-out: 보통-느리게<br>
+ ease-in-out: 천천-보통-천천

<br/>
<br/>


## 카드 뒤집기 애니메이션



![bandicam2024-10-0201-13-53-953-ezgif com-video-to-gif-converter](https://github.com/user-attachments/assets/64000f1b-7d13-4155-80ee-1dbc7855652d)<br/>
![flip](https://github.com/user-attachments/assets/b689327a-b5da-4841-b86a-5d87714073ec)<br/>
![flip2](https://github.com/user-attachments/assets/7e4d0619-f6fa-4f0f-8064-c2c6bd6ee5eb)<br/>

마우스 호버 시 카드를 뒤집어 앞면에서 뒷면으로 전환하는 효과를 구현하였다.<br/>

+ transform-style: preserve-3d
  transform-style은 3D 공간에서 자식 요소들을 렌더링하는 방법을 결정하는데, 기본값은 flat(납작한)이다.
  이와 반대로 3D 렌더링을 결정하는 값이 preserve-3D으로, 이를 사용하면 해당 컨테이너 영역을 삼차원 영역으로 활용할 수 있다.

+ transform: rotateY(180deg)는 카드를 y축 기준으로 180도 회전시키는 3D 변환을 의미하고, 결과적으로 앞면이 사라지고 뒷면이 보이게 된다.

+ backface-visibility: hidden은 카드를 뒤집었을 때 카드의 앞면이 보이지 않도록 설정한다. 이 속성이 없으면 회전 시 앞면과 뒷면이 동시에 보일 수 있다.

