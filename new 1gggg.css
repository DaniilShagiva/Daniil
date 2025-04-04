* {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
.gallery img {
  -webkit-transition: all .3s ease-in-out;
  -moz-transition: all .3s ease-in-out;
  transition: all .3s ease-in-out;
}
.gallery img {
  max-width: 100%;
}
.gallery .mainImg {
  position: relative;
  margin-bottom: 15px;
}
.gallery .mainImg img {
  display: block;
  margin: auto;
}
.gallery .mainImg i {
  color: #fff8dc;
  width: 20px;
  height: 20px;
  display: flex;
  justify-content: center;
  align-items: center;
  position: absolute;
  top: 50%;
  -webkit-transform: translateY(-50%);
  -moz-transform: translateY(-50%);
  transform: translateY(-50%);
  cursor: pointer;
}
.gallery .mainImg i.fa-chevron-left {
  left: 0;
}
.gallery .mainImg i.fa-chevron-right {
  right: 0;
}
.gallery .thumbnails {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: space-between;
}
.gallery .thumbnails li {
  cursor: pointer;
}
.gallery .thumbnails li:not(:last-child) {
  margin-right: 5px;
}
.gallery .thumbnails li img {
  border: 2px solid #CCC;
  padding: 2px;
  background-color: #fd5e53;
  opacity: .8;
}
.gallery .thumbnails li img.active {
  border-color: #0a4500;
  opacity: 1;
}
$(function () {
  'use strict';
  
  $('.mainImg').height($('.mainImg img').height());
    $('.thumbnails img').click(function () {
    $(this).addClass('active').parent().siblings().find('img').removeClass('active');
    $('.mainImg img').hide().attr('src', $(this).attr('src')).fadeIn(300);
  });
    $('.mainImg i').click(function () {    
    if ($(this).hasClass('fa-chevron-right')) {
      console.log('right');
      if ($('.thumbnails .active').parent().is(':last-of-type')) {
        $('.thumbnails .active').parent().parent().find('li:eq(0)').find('img').click();
      } else {
        $('.thumbnails .active').parent().next().find('img').click();
      }
    } else {
      console.log('left');
      if ($('.thumbnails .active').parent().is(':first-of-type')) {
        $('.thumbnails .active').parent().parent().find('li:last-of-type').find('img').click();
      } else {
        $('.thumbnails .active').parent().prev().find('img').click();
      }
    }
  });
});
