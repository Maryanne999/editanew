
$(document).ready(function(){
  $('.banner-slider.js-banner-slider').slick({
        prevArrow: '<button type="button" class="slick-prev"><i class="fa fa-angle-left" aria-hidden="true"></i></button>',
        nextArrow: '<button type="button" class="slick-next"><i class="fa fa-angle-right" aria-hidden="true"></i></button>',
        slidesToShow: 1,
        slidesToScroll: 1,
        autoplay: true,
        autoplaySpeed: 5000,
        infinite: true,
        draggable: false

    }
  );
});
    $('.js-slide-carousel').slick({
        prevArrow: '<button type="button" class="slick-prev"><i class="fa fa-angle-left" aria-hidden="true"></i></button>',
        nextArrow: '<button type="button" class="slick-next"><i class="fa fa-angle-right" aria-hidden="true"></i></button>',
        slidesToShow: 3,
        slidesToScroll: 1,
        swipeToSlide: true,
        infinite: true,
        responsive: [
      {
        breakpoint: 767,
        settings: {
          slidesToShow: 2
        }
      },
      {
        breakpoint: 480,
        settings: {
          slidesToShow: 1
        }
      }
    ]

    });



$(document).ready(function(){

      var headerInner = $('.page-header');
      var mobileNav = $('.menu-nav');

      $(window).scroll(function () {
           if ( $(this).scrollTop() > headerInner.height() ) {
               mobileNav.addClass("menu-nav--fixed");
               // headerInner.css('margin-bottom', '40px');
           } else {
              if ( $(this).scrollTop() <= headerInner.height() ) {
                mobileNav.removeClass("menu-nav--fixed");
                // headerInner.css('margin-bottom', '0');
            }
          }

       });//scroll

	     var currItem;
  // $('.sub-nav:not(:first-child)').css("display", "none");
    $('.header-bottom-nav__item').on('mouseenter', function () {
    currItem = 0;
    $('.sub-menu__link').removeClass('sub-menu__link--curr');
    $('.sub-menu__item:first-child .sub-menu__link').addClass('sub-menu__link--curr');
    $('.sub-menu').css("display", "none");
    $('.sub-menu:first-child').fadeIn();
  });
  $('.sub-menu__link').on('mouseenter', function () {
    if (currItem == ($(this).data('nav'))) {
      return false;
    } else {
      $('.sub-nav').css("display", "none");
      $('.sub-menu__link').removeClass('sub-menu__link--curr');
      currItem = $(this).data('nav');
      $(currItem).fadeIn();
      $(this).addClass('sub-menu__link--curr');
    }

  });

   });

       // mmenu initialization
          $('#mobile-menu').mmenu({
             // options
          // }, {
             // configuration
             offCanvas: {
                pageNodetype: "#wrapper-content"
             },
             extensions: ["position-right"]

          });

      var API = $("#mobile-menu").data( "mmenu" );
      $("#cross-btn").click(function(evt) {
        evt.preventDefault();
         API.close();
      });
