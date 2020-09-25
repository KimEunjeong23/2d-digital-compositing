# This is Week03 class Assignment
## Color space
### What is color space?
Color Space 색공간

색의 3요소를 이러한 특성에 근거해 하나의 중심축을 기준으로 색을 원형으로 배치하고, 수직 방향으로 명도에 따른 변화를, 중심축으로부터의 수평 거리를 이용해 채도 변화에 따른 차이를 표현하면 원통 형태의 3차원 색 좌표를 만들 수 있다. 이렇게 색을 공간 좌표에 나타낸 것을 ‘색공간(color space)’이라고 한다.  <sup>1)</sup>

### 다양한 색공간 

- CIE Lab 색공간 <sup>2)</sup>

인간이 색채를 감지하는 노랑-파랑, 초록-빨강의 반대색설에 기초하여 CIE에서 정의한 색 공간이다.

###### 국제조명위원회(CIE, Commission Internationale de I'Eclairage)

(1) L*: 반사율(인간의 시감과 같은 명도)을 나타내며, 0~100까지의 단계로 소수점 이하 단위도 표현할 수 있다.

(2) a*: 색도 다이어그램으로 ＋a*는 빨강, -a*는 초록 방향을 나타낸다.

(3) b*: 색도 다이어그램으로 ＋b*는 노랑, -b*는 파랑 방향을 나타낸다.


![Lab](https://user-images.githubusercontent.com/70870803/94282167-77480600-ff8a-11ea-80a2-335958d600d2.jpg)

###### <그림1> CIE Lab 색공간

 - YUV 
 
컬러 영상을 구현하는 방법으로 밝기는 Y로 청색의 색차는 U로 적색의 색차는 V로 색을 표현하는 방식이다.
YUV는 영상신호를 휘도(luminance)와 색차 신호(chrominance)로 구성하는 컴포넌트(component) 신호이다. <sup>3)</sup>

사람의 눈이 민감하게 반응하는 밝기값(luma)과 상대적으로 덜 민감한 색상값(chrominance)을 분리해 신호 처리를 수행하는 색공간으로 색상값 없이 밝기값만을 사용하면 바로 흑백 영상을 얻을 수 있기 때문에 컬러와 흑백 장비가 섞여 있어도 쉽게 호환성을 확보할 수 있다는 장점이 있다.
또한 밝기값과 색상값의 데이터 밀도를 다르게 사용하는 것도 가능하기 때문에 영상신호의 크기를 효과적으로 절약(압축)하는 것이 가능해진다. <sup>4)</sup>

- YCbCr/YPbPr <sup>5)</sup>

근본적으로 YUV와 같은 원리를 사용하는 YCbCr은 절대값을 갖는 색공간이 아니며 RGB 정보를 변환 및 압축하는 방식의 하나이다.
YCbCr과 YPbPr은 근본적으로 같은 것으로 YCbCr은 디지털에서 YPbPr은 아날로그 시스템에서 사용하는 방식이다. 


- sRGB(standard RGB) 

HP와 마이크로소프트(Microsoft)에서 제안한 컴퓨터를 위한 RGB 색공간으로 HDTV 시스템에서 사용하는 Rec.709와 동일한 개머트를 갖는 색공간이다.<sup>6)</sup>
색상을 표현할 수 있는 영역이 좁다는 단점이 있다.

- ACES Colorspace

The Academy Color Encoding System 에서 제안한 색 공간이다. 색보정 단계마다 혼란을 방지하고 다양한 컬러를 표용하기 위해 개발되었다.

### Color Gamut

전체 태양 빛의 영역인 외곽선에서 각각의 매체가 재현할 수 있는 색 공간 영역이다. <sup>7)</sup>

![image001](https://user-images.githubusercontent.com/70870803/94286859-89c53e00-ff90-11ea-9aef-e7f0f03c4643.jpg)

###### <그림2> Color Gamut comparison

- Rec.709는 sRGB와 유사하다.

- Rec.2020는 SDR과 넓은 색역(WCG), 해상도, 프레임레이트, 색깊이, 컬러, 휘도-색도 컬러표현, 크로마 서브샘플링과 감마보정 등을 포함한 초고선명 텔레비전(UHD TV)의 여러가지 측면을 정의한다.<sup>8)</sup>

- DCI-P3 미국 영화 산업의 디지털 영화 프로젝션을 위한 일반 RGB 색 공간이다. <sup>9)</sup>

## Gamma / Linear workflow
### What is Gamma/ Linear?  <sup>10)</sup>

Gamma는 실제 색이 아닌 사람이 자연스럽게 느끼는 색을 만들어낸다. 그로인해 화질이 향상되는 효과를 주기 위함이다.

Linear은 실제의 색을 표현한다. 왜곡되지 않은 선.

![Gamma-Signal-v01](https://user-images.githubusercontent.com/70870803/94294389-b9794380-ff9a-11ea-82cc-25c57e2b089c.jpg)
###### <그림3> Gamma 
Linear한 상태를 gamma correction을 통해 밝게 연산하여 gamma 공간으로 이끈 후, 다시 어둡게 연산하여 Linear한 상태를 만든다.

## Color Correction
비디오 필름이나 디지털 이미지의 색을 조정하는데 쓰는 일련의 기술을 가리키는 국제적인 용어이다. <sup>11)</sup>

- default

아무 색상이 변하지 않은 상태.

- offset

모든 이미지의 밝기를 올리거나 낮춤.

- Gain

로우레벨을 고정시킨 상태에서 하이라이트만 조정할 때 사용.

- Gamma 

로우톤과, 하이라이트 톤을 고정시킨 상태로 미들톤을 조정.

- Contrast 

이미지의 대비를 줄 때 사용.

- Clamp

특정 색영역을 잘라내기 위해서 사용. 영역은 보통 사용자가 설정한다.  <sup>12)</sup>


## What is LUT?
 룩업 테이블(lookup table)은 컴퓨터 과학에서 일반적으로 배열이나 연관 배열로 된 데이터 구조로, 런타임 계산을 더 단순한 배열 색인화 과정으로 대체하는 데 자주 쓰인다. <sup>13)</sup>
 
 비디오에 적용하여 룩을 변경할 수 있는 고정된 숫자 값의 테이블이다. 이미지의 대비 또는 색상을 변경하거나 둘 다 변경할 수 있다.
 
 LUT를 사용하는 주된 목적은 Log를 Rec.709로서의 변환속도를 단순화하기 위해서이다. 
 
 1D LUT는 입력값과 출력값이 1:1로 매칭되는 가장 간단한 테이블이다.<sup>14)</sup>
 
 3D LUT는 3차원 cube 공간의 좌표값으로 HUE, Saturation 까지 표현이 가능하다. <sup>15)</sup>

![3D LUT](https://user-images.githubusercontent.com/70870803/94299603-d7e33d00-ffa2-11ea-8cd0-b993075e4b6d.JPG)

###### <그림4> 3D LUT

## Logspace / sRGB

#### Log color curve

현재 거의 모든 카메라 제조 업체는 자체 로그 곡선을 제조한다. 

S-Log 2&3 (Sony), LogC (Arri), Canon Log, V-Log (panasonic), Red Logfilm, Blackmagic Log, etc. 

#### WHY WE USE? 

The biggest reason to use the Log color curve is how it retains the most dynamic range of information from the camera sensor (or film negative).  <sup>16)</sup>

#### Comparison
![Log-Curve](https://user-images.githubusercontent.com/70870803/94302753-afaa0d00-ffa7-11ea-8fa1-25c771858ac7.jpg)
###### <그림5> Linear curve, Log curve

![sRGB---](https://user-images.githubusercontent.com/70870803/94302763-b46ec100-ffa7-11ea-942a-25d288905f04.jpg)
###### <그림6> sRGB curve

![Log-Curve ---](https://user-images.githubusercontent.com/70870803/94302771-b769b180-ffa7-11ea-8b4f-9886f223f063.jpg)
###### <그림7> Log curve

###### 포토샵 8bit-16bit

sRGB 이미지를 변환하는 과정에서 손실이 일어날 수도 있다.

Log는 흰색 및 검은색 영역의 값을 압축하여 저장하는데 필요한 공간을 최소화한다.


### 출처
<sup>1)</sup> <sup>4)</sup> <sup>5)</sup> <인터넷 자료> https://terms.naver.com/entry.nhn?docId=3340383&cid=58161&categoryId=58161

<sup>2)</sup> <인터넷 자료> https://terms.naver.com/entry.nhn?docId=271068&cid=42641&categoryId=42641

<sup>3)</sup> <인터넷 자료> https://terms.naver.com/entry.nhn?docId=2070766&cid=42346&categoryId=42346

