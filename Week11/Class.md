# Tracking in NUKE
## 1point tracker
- tracker node 사용
빨간 버튼 > 트래킹 할 영역을 선택한 후, 위의 재생 버튼을 누르면 자동으로 트래킹이 됨. 
<img width="774" alt="스크린샷 2020-11-20 오후 1 04 39" src="https://user-images.githubusercontent.com/70870803/99759568-f7778b80-2b35-11eb-9e31-a1f2c04a0feb.png">

중간에 튕긴 부분 직접 다시 설정.

tracker node 안에 있는 export 부분에서 Transform(Match-move)create.

Merge node 사용하여 완성.

## 2point tracker
- 앞선 1point와 유사
- 상하좌우로 움직임이 많은 영상에.

add track하여 두개의 포인트 생성

2개 트랙 T,R 체크.> 2개 동시 선택 후, tracker node 안에 있는 export 부분에서 Transform(Match-move)create.

Merge node

<img width="585" alt="스크린샷 2020-11-20 오후 1 17 25" src="https://user-images.githubusercontent.com/70870803/99759581-04947a80-2b36-11eb-8a72-374573321bbe.png">

## 3point tracker
- 3개의 포인트

## 4point tracker
- 4개의 포인트
- 컴퓨터 스크린 같은거에 활용하기 좋음.

1. 4개의 포인트를 지정해서 트랙킹 설정하기
2. 교체할 footage에 ConerPin2D node 생성
3. ~ > Link to . 사각형 모서리 부분 맞추기.


## Planar tracker
- roto를 활용

- 간판 같은거 갈아끼우기 좋음

Planar tracker node생성 > roto > perspective 맞추기 > roto 안의 tracking 에서 ConerPin2D(absolute) create > From에서 set to input 눌러 사이즈 맞추기.

conerPin2D는 footage와 연결

merge node로 마무리

<img width="377" alt="스크린샷 2020-11-20 오후 1 34 14" src="https://user-images.githubusercontent.com/70870803/99759587-09f1c500-2b36-11eb-8084-c54737636eef.png">
노드 예시

## Color Match
본래의 화면과 새로운 이미지를 자연스럽게 합성하기 위해서는 컬러매치가 필요하다.

- Grade node 를 사용해 RGB를 맞춘다.
- Edge blur node 를 사용해 모서리에 블러를 넣어 자연스러운 효과.
- Grain node 를 사용해 노이즈를 삽입해 주변과 맞춘다.


