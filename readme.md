1. fill: The fill property is used for setting the color of an SVG shape. It accepts any color value.
2. box-shadow(x, y , độ đâm nhạt của bóng , màu)
3.object-fit: contain;
4. display: block; phải đi với thẻ khác hoặc block text-align: center;
5. 

@keyframes scale {
  0% {
    transform: scale(.5);
  }

  100%{
    transform: scale(1);
  }
}

6. Cách tạo mũi tên

.header-notice::before {
    content: '';
    position: absolute;
    display: block;
    z-index: 3;
    border-left: 15px solid transparent;
    border-right: 15px solid transparent;
    border-bottom: 15px solid rgb(255, 255, 255);
    top: -13PX;
    right: 10px;
}


7. cách tạo before để hover
.nav-qr::before {
  content: '';
  display: block;
  position: absolute;
  width: 80px;
  height: 30px;
  background-color: transparent;
  z-index: 4;
  top: -15px;
}

8. focus của thẻ input(có đấu cộng nha)
.header-form-search input:focus + .header-serch-hint {
  display: block;
}

9.box-sizing: border-box; 
{
  
    padding + content
}

10. left top right - bt sẽ không hoạt động trên elements ko có position
11. margin sẽ tạo khoảng hông xung quanh element ngoài boder 
+ margin-top: 0px sẽ lấy vị trí tốp của thăng cha overflow trên thằng cha sẽ ẩn thằng con đi

12. sự khác nhau giữa querySelector và getElementbyClassName

13. sự đặc biệt của transform là gì ? Sự khác nhau giữu trasition và transform
chúng ta đã biết Transition giúp ta điều khiển được các thuộc tính CSS tác động lên các đối tượng cho "mượt" trong 1 khoảng thời gian. Transforms thì không giúp điều khiển các thuộc tính tác động lên đối tượng mà sẽ điều khiển trực tiếp đối tượng đó, như là div, image,...

13. phần trăm trong transform: translateY(-50%) là độ dài y của chính phần tử đó (translate: sự biến dạng)

14. Tỷ lệ khung hình là gì ?

15. cách tạo card với tỉ lệ khung hình
.product-container {
  margin-top: 10px;
  aspect-ratio: 1/1;
 background-color: red;
}

.product-container__img {
  aspect-ratio: 1/1;
  background-repeat: no-repeat;
  background-position: center center;
  background-size: contain;
}
