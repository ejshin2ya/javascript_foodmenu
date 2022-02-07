## 1. 구현한 내용
* 원하는 메뉴를 클릭하면 listDiv 구역에 사진을 띄워준다.
* 랜덤버튼 클릭시 랜덤으로 오늘의 메뉴 추천
* 메뉴 클릭할때마다 음식 이미지 사진에 맞게 메뉴명도 변경해준다.
* 마우스를 올리기 전에는 불투명했던 음식 사진이 마우스를 올리면 사진이 선명해지면서 테두리가 생긴다.

## 2. 구현한 기능
* let, querySelector, addEventListener를 사용하여 클릭(click) 이벤트 발생하면, listDiv에 음식 이미지를 append하여 가운데 위치에 이미지를 출력한다.
* Math.floor(Math.random()*4)를 사용하여 0~3까지의 랜덤한 숫자를 나오게 하였다. 랜덤한 숫자는 imgArr라는 리스트의 index에 해당하며, 리스트의 값은 음식 이미지의 src 위치값을 담고 있다. setAttribute로 이미지 주소, 이미지 크기를 지정 후 listDiv에 append하여 특정 공간에 이미지 출력.
* text.innerText를 사용하여 클릭 이벤트 발생시에 text값도 변경해준다.
* img의 opacity(불투명도)를 0.5로하여 불투명한 상태로 만들었다. hover는 마우스를 올렸을때 효과를 줄수 있는 기능으로 opacity를 1로 지정하여 음식 사진이 투명해지도록 하였다. 또한, hover에 boader : 10px solid color를 지정하여 이미지 사진에 테두리 생성기능 구현  
