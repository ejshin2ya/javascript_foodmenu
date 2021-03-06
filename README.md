## 1. 구현한 내용
* 원하는 메뉴를 클릭하면 listDiv 위치에 메뉴에 해당하는 사진을 가운데 정렬하여 보여준다.  
* 랜덤버튼 클릭시 랜덤으로 오늘의 메뉴 추천
* 메뉴 클릭할 때마다 음식 이미지에 해당하는 글자가 표시되도록 텍스트 변경.
* 마우스를 올리기 전에는 불투명했던 음식 사진이 마우스를 올리면 사진이 선명해지도록 함, 또한 마우스 올리면 사진 주변에 테두리가 생기도록 구현.

## 2. 구현한 기능
* let, querySelector, addEventListener를 사용하여 클릭(click) 이벤트 발생하면, listDiv에 음식 이미지를 append하여 웹페이지에 사진을 띄우는 동적 기능 구현. 
  display:block, margin:auto를 사용하여 사진을 가운데 정렬함. 
* Math.floor(Math.random()*4)를 사용하여 0~3까지의 랜덤한 숫자를 나오게 하였다. 랜덤한 숫자는 imgArr라는 리스트의 index에 해당하며, 리스트의 값은 음식 이미지의 src 위치값을 담고 있다. setAttribute로 이미지 주소, 이미지 크기를 지정 후 listDiv에 append하여 특정 공간에 이미지 출력.
* text.innerText를 사용하여 클릭 이벤트 발생시에 text값도 변경해준다.
* img의 opacity(불투명도)를 0.5로하여 불투명한 상태로 만들었다. hover는 마우스를 올렸을 때 효과를 줄수 있는 기능으로 opacity를 1로 지정하여 음식 사진이 선명해지도록 하였다.(불투명도 제거) 또한, hover에 boader : 10px solid color를 지정하여 이미지 사진에 테두리 생성기능 구현, justify-content:space-around를 적용하여 가로축 여백을 균일하게 사용하는 flex 기능 활용.
