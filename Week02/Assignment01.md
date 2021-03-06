# This is Week02 class Assignment 01
## What is color & digital color?
### 색의 정의와 종류

#### What is color?

색은 다양한 파장의 에너지로 이루어져 있고, 그 에너지가 우리의 동공을 지나 안구 속의 망막에 도달하면 신경 신호로 변환되어 최종적으로 뇌에서 처리된다.
색은 색조, 채도, 명도 3가지 속성을 지닌다. <sup>1)</sup>

1. 색조(Hue)- 색상환 내에서의 위치를 말한다. 빨강, 노랑, 초록, 파랑 등 어떤 색과 다른 색을 구별하는 고유한 속성이라고 할 수 있다.

![색상환](https://user-images.githubusercontent.com/70870803/93597174-96c4b900-f9f5-11ea-9cd4-d74f6c591064.jpg)
  
######  <그림1> 먼셀의 색상환




2. 채도(Saturation)- 색의 순수하고 선명한 정도. 채도가 높을수록 눈에 띈다. 

![채도](https://user-images.githubusercontent.com/70870803/93597431-033fb800-f9f6-11ea-99c6-b03f7e9c3ce4.JPG)
  
######  <그림2> 채도의 예시




3. 명도(Value)- 색의 밝고 어두운 정도. 명도가 ‘어둡다, 밝다’로 표현이 가능하다. 

![명도](https://user-images.githubusercontent.com/70870803/93597440-05a21200-f9f6-11ea-9bba-85f23f4f4e90.JPG)
  
######  <그림3> 명도의 예시



#### What is digital color?

디지털 컬러란, 디지털 신호에 의해 만들어진 색채 표현 방법이다. 
최소의 단위는 비트(Bit)이며, 비트 수는 디지털 색 수를 결정한다. 
컴퓨터의 모니터는 빛의 3원색인 빨강, 파랑, 초록의 전자총에서 발사되어 형광에면에 부딪쳐 색을 나타낸다. 
작은 점(비트)이 모여 화소(Pixel픽셀)를 나타내며 화소는 디지털 이미지의 최소 단위로 이미지의 선명도와 질선명도을 결정짓는 요소로 픽셀 수에 의해 차이가 나게 된다. <sup>2)</sup>

![RGB](https://user-images.githubusercontent.com/70870803/93599723-8b738c80-f9f9-11ea-8f9a-01ddfc2d1a86.JPG)

######   <그림4> 모니터를 확대해보면.


#### Many types of explain color

1. RGB color model

3원색 모델이란, RGB는 빨강(red), 초록(green), 파랑(blue)의 약어. 이 3색을 기본으로 하여 구성되는 하드웨어 지향적인 색 모델로 일반적인 컬러 TV 모니터에 사용된다. <sup>3)</sup>

About RGB

빨간색(R), 초록색(G), 파란색(B)을 모두 섞으면 – 흰색 (가산혼합) 
세 가지 색 중 아무 색도 비추지 않으면 – 검은색

![RGB_](https://user-images.githubusercontent.com/70870803/93600689-ff626480-f9fa-11ea-9509-2b2009a665cb.JPG)

######   <그림5> RGB


예시)
| RGB(R,G,B)       |  색                         | 
| ---------------- |:---------------------------:|
| RGB(255,0,0)     | 빨간색                       | 
| RGB(255, 100, 0) | 초록색이 조금 섞인 연한 빨간색 |
| RGB(0,255,0)     | 초록색                       |
| RGB(0,0,255)     | 파란색                       |
      
######   <표1> RGB 색 예시      
      
모니터의 화면은 화소라고 불리는 아주 작은 사각형이 여러 개 모여서 만들어진 것이다. 
각 화소는 빨간색, 녹색, 파란색 세 가지의 조합으로 만들어진다.
화소 하나마다 바이트(byte)라는 단위를 이용하여 각각 빨간색 1바이트, 초록색 1바이트, 파란색 1바이트가 들어가게 된다. 그리고 1바이트는 0부터 255까지 256단계의 색을 나타낼 수 있다. <sup>4)</sup>

2. CMYK

C(시안), M(마젠타), Y(노랑), K(검정)의 4색을 조합해서 정의한 색.
주로 인쇄에서 사용된다. <sup>5)</sup>

![CMYK](https://user-images.githubusercontent.com/70870803/93600697-01c4be80-f9fb-11ea-9672-d1fb446e2e60.JPG)

######   <그림6> CMYK
   

3. H/S/B

컴퓨터 그래픽스(CG)에서 색을 기술하는 데 사용되는 색 모델의 하나인 색상·채도·명도 모델. 
H는 색원상의 색인 색상(hue)를 뜻한다.

0도에 적색, 60도에 황색, 120도에 녹색, 180도에 시안(청록색), 240도에 청색, 300도에 마젠타(적보라색)가 있다. 

S는 채도(saturation)를 뜻한다. 어떤 특정 색상의 색의 양으로 보통 0~100%의 백분율로 나타낸다. 

B는 명도(brightness)를 뜻하는데, 어떤 색 중 백색의 양으로 0%이면 흑이고 100%이면 백이다. 

HSB 모델을 HLS, 즉 색상-명도-채도 모델이라고도 한다. <sup>6)</sup>


4. L/a/b

인간 감성에 접근하기 위하여 연구된 결과로 인간이 색채를 감지하는 노랑-파랑, 초록-빨강의 반대색설에 기초하여 CIE에서 정의한 색 공간. 
이 색 공간은 조색을 할 때 색채의 오차 범위와 방향을 쉽게 짐작케해 세계적으로 가장 널리 통용되고 있다. 

(1) L*: 반사율(인간의 시감과 같은 명도)을 나타내며, 0~100까지의 단계로 소수점 이하 단위도 표현할 수 있다.

(2) a*: 색도 다이어그램으로 ＋a*는 빨강, -a*는 초록 방향을 나타낸다.

(3) b*: 색도 다이어그램으로 ＋b*는 노랑, -b*는 파랑 방향을 나타낸다. <sup>7)</sup>


![Lab](https://user-images.githubusercontent.com/70870803/93602352-7a2c7f00-f9fd-11ea-8dd3-a1d39b588011.jpg)

######   <그림7> Lab 색공간
   
   
## What is Alpha?
### 알파의 뜻과 유래

#### What is Alpha?

이미지의 특정 영역을 가리거나(마스크) 제어하는 특수한 채널이다. 
일반적인 화면은 3개의 채널로 구성되는데 R(red), G(green), B(blue)의 3개의 빛을 합성하여 이미지를 만든다. 
이 3개의 채널 외 4번째 채널을 알파 채널이라고 하는데 다른 이미지와 합성하는 채널로 흑, 백으로 되어있다. 

보통 흰색은 불투명하다는 뜻이고 검은색은 투명하다는 뜻이다.

예를 들어, 알파 채널이 가진 이미지를 A, 합성될 화면을 B라고 하고, 
A화면이 가지는 알파 채널의 흰색 부분은 A의 이미지가 나타나고 검은 부분은 투명하게 되어 뒤 배경에 해당하는 B의 이미지가 나타나게 된다. <sup>8)</sup>

straight alpha.(unassociated) 

premultiplied alpha.(associated)

#### Who made it?

Ed Catmull와 Alvy Ray Smith가 1970년대에 New York Tech에서 Alpha의 개념을 발명했다.
1984년에 Thomas Porter와 Tom Duff에 의해 완전히 발명되었다.


#### 출처
<sup>1)</sup>
              
              <국내단행본> 양소영 외 8명, 음악미술 개념사전, 2010. 7. 12.

              <인터넷 자료> https://www.youtube.com/watch?v=0DXZvcfPVrk

<sup>2)</sup> 

              <국내단행본> 박연선, 색채용어사전, 국립국어원,  2007.

<sup>3)</sup> 

              <국내단행본> 전산용어사전편찬위원회, 컴퓨터인터넷IT용어대사전, 일진사, 2005.

<sup>4)</sup> 
              
              <인터넷 자료> https://terms.naver.com/entry.nhn?docId=3607526&cid=58598&categoryId=59316

<sup>5)</sup> 
              
              <국내단행본> 박연선, 색채용어사전, 국립국어원,  2007.

<sup>6)</sup> 
              
              <국내단행본> 한국정보통신기술협회, IT용어사전

<sup>7)</sup> 
              
              <국내단행본> 이강원, 손호웅, 지형 공간정보체계 용어사전 ,2016. 1. 3.

<sup>8)</sup> 
              
              <국내단행본> 김일태 외 4명, 만화애니메이션사전, 2008. 12. 30.
              
#### 이미지 출처

              <그림1> http://art-design-glossary.musabi.ac.jp/hue-circle/
              <그림2> https://blog.naver.com/differentn/80129513141
              <그림3> 박연선, 색채용어사전, 국립국어원,  2007.
              <그림4> https://www.youtube.com/watch?v=T0jzClmP2pc
              <그림5> <그림6> https://www.shutterstock.com/ko/image-vector/rgb-cmyk-color-mixing-vector-diagram-1090078490
              <그림7> https://terms.naver.com/entry.nhn?docId=271068&cid=42641&categoryId=42641
