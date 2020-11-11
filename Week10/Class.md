# CHROMA KEY in NUKE
## Greenscreen

### Denoise node
- 이미지의 노이즈를 줄여주는 기능
1. 노드 생성 후 에러
2. 어느 부분을 denoise할 것인지 선택하면 에러가 없어짐.

### Keymix node
영역별로 key node 관리 가능

### Despill
#### Core despill
- 피사체에 반사된 초록색 부분으 지우는 방법
keylight node

Hue correct- 영역 선택 후, green값 낮추기
<img width="586" alt="스크린샷 2020-11-12 오전 12 17 38" src="https://user-images.githubusercontent.com/70870803/98832366-12843480-2480-11eb-9dcd-4550d1d3d1a4.png">
#### Edge despill

