# Rotoscoping & Color match in NUKE

## 동영상이나 사진 첨부
- 동영상 첨부 시, error가 발생하는 경우!
adobe Media Encoder에서 dpx, jpg로 전환하기.

## Roto
tab키 누른 후, roto 입력 혹은 단축키 O


<img width="1440" alt="스크린샷 2020-11-03 오후 10 30 12" src="https://user-images.githubusercontent.com/70870803/97991798-3c58ae00-1e25-11eb-9430-f014785e1375.png">

roto 따고 싶은 피사체의 외곽을 따라 따기. 

<img width="1397" alt="스크린샷 2020-11-03 오후 10 42 32" src="https://user-images.githubusercontent.com/70870803/97992710-69599080-1e26-11eb-8dd3-331771cc3bd0.png">

이런식으로? 따면 된다. (더 깔끔하고 섬세하게..)

확대해서 섬세하게.

머리, 몸통, 팔로 나누어 이름을 저장하면 더욱 편하다.

Merge 사용하여 배경과 합치기> A over B

## Color Match

#### 컬러 매치를 위한 순서

1. contrast

- Grade 노드 

1.1 Black -- offset

1.2 White -- Gain

1.3 Midtone -- Gamma

2. Saturation
- Saturation 노드

3. Color temperature (Kelvin)
- Grade 노드

<img width="87" alt="스크린샷 2020-11-03 오후 10 14 25" src="https://user-images.githubusercontent.com/70870803/97993614-a7a37f80-1e27-11eb-9eb3-5c3514d6447b.png">



