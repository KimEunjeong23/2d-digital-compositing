# Tracking in NUKE
## 1point tracker
- tracker node 사용
트래킹 할 영역을 선택한 후, 버튼을 누르면 자동으로 트래킹이 됨. 

tracker node 안에 있는 export 부분에서 Transform(Match-move)create.

Merge node 사용하여 완성.

## 2point tracker
- 앞선 1point와 유사
- 상하좌우로 움직임이 많은 영상에.

add track하여 두개의 포인트 생성

2개 트랙 T,R 체크.> 2개 동시 선택 후, tracker node 안에 있는 export 부분에서 Transform(Match-move)create.

Merge node

## 3point tracker
- 3개의 포인트

## 4point tracker
- 4개의 포인트
- 컴퓨터 스크린 같은거에 활용하기 좋음.

1. 4개의 포인트를 지정해서 트랙킹 설정하기
2. Tracker node 아래에 (Export>ConerPin2D)생성
3. 교체할 footage에 ConerPin2D node 생성
