# CHROMA KEY in NUKE
## Greenscreen
### NODE


#### 자주 사용하는 노드
1. Keyer

A,B,C,D 조절

Keyer에 대한 자세한 사용방법: http://learn.foundry.com/nuke/12.2/content/reference_guide/keyer_nodes/keyer.html?cshid=Keyer

2. Hue Keyer
3. Difference
4. Keylight

- Screen color 설정> 검정 네모 박스 누르고, (control키 누른채로 그린스크린 한 부분)or (command키 누른채로 그린스크린 한 부분 선택)
- Screen color matte에서 Clip balck 조절하기 

<img width="573" alt="스크린샷 2020-11-03 오후 9 16 12" src="https://user-images.githubusercontent.com/70870803/97988700-b89cc280-1e20-11eb-95a3-fd166361bb21.png">


5. Ultimatte (NUKE non-commercial에서 사용 불가 ㅜㅜ)
6. Primatte  (NUKE non-commercial에서 사용 불가)
7. IBKGizmov3
8. IBKColourv3


#### 그린스크린에 다른 배경 합성

이미지 or 영상과 Merge

A(greenscreen footage) over B(background)
