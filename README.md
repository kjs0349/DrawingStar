# DrawingStar
 별 그리는 애니메이션을 만들어 봤습니다.

css animation을 이용해 별을 그려보았어요!

특정 영역에 마우스를 올려 놓으면 그려지는 형식으로 만들어 보았습니다

우선 선을 다섯개 만들고 
특정 영역에 position: relative를 주고 
선들에 position: absolute를 주어 
선마다 시작 위치를 지정해 주고
transform: rotate()를 통해 각도를 돌려주었습니다 
transform: rotate()는 기본적으로 center 기준으로 돌아가서 
각도 맞추기가 어려워 transform-orgin으로 
선마다 기준점을 다르게해서 원하는 방향으로 돌렸습니다.
그리고 높이 값을 가지고 있지 않다가 hover 하면 높이 값을 주고
transition 속성을 통해 자연스럽게 긋는 모습을 연출하였고 
선마다 딜레이를 주어 순서대로 그려지게 하였습니다.
transform: rotate()를 통해 돌려 주었는데 이 돌아가는 모습까지 표현되어 자연스럽게 그려지지 않아 
@keyframes 0%에 transform-origin값과 transform: rotate()값을 주어 돌아간 위치에서 바로 실행되게 만들었습니다.
