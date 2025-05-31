<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Yaad Yaad Aati Hain</title>
    <link href="https://fonts.googleapis.com/css2?family=Kumbh+Sans&display=swap" rel="stylesheet"> 
    <!-- https://fonts.google.com/specimen/Kumbh+Sans -->
    <link rel="stylesheet" href="fontawesome/css/all.min.css">  <!-- https://fontawesome.com/-->  
    <link rel="stylesheet" href="css/magnific-popup.css">       <!-- https://dimsemenov.com/plugins/magnific-popup/ -->
    <link rel="stylesheet" href="css/tooplate-vertex.css">

<style> 

    .container-lg, .container-lg.px-3.my-5.markdown-body {
        /* width: 100% !important;
        margin: 0 auto !important; */
        display: contents;
    }
</style>
</head>
<body>
    <!-- Page Loader -->
    <div id="loader-wrapper">
        <div id="loader"></div>

        <div class="loader-section section-left"></div>
        <div class="loader-section section-right"></div>

    </div>

    <!-- Site logo -->
    <h1 class="tm-brand">
        <marquee class="tm-ty-text">Thanks! For Visting! </marquee>
        <marquee class="tm-brand-text">Follow for more!</marquee>
    </h1>

    <!-- Nav -->
    <nav class="tm-nav">
        <button class="navbar-toggler" type="button" aria-label="Toggle navigation">
            <i class="fas fa-bars"></i>
        </button>
        <ul id="tm-main-nav">
            <li class="nav-item">                                
                <a href="#intro" class="nav-link current">
                    Home
                </a>
            </li>
            <li class="nav-item">
                <a href="#services" class="nav-link">
                    Book Published
                </a>
            </li>
            <li class="nav-item">
                <a href="#gallery" class="nav-link">
                    Achievement 
                </a>
            </li>
            <li class="nav-item">
                <a href="#about" class="nav-link">
                   About YYAH 
                </a>
            </li>
            <li class="nav-item">
                <a href="#contact" class="nav-link">
                    Contact
                </a>
            </li>
        </ul>
    </nav>

   <main>
       <div>sher is back</div>
   </main>

    <script src="js/plugins.js"></script>
    <script>
        $(window).on("load", function() {
            $('body').addClass('loaded');
        });

        $(function(){
            
            /*************** Navigation *****************/

            const tmMainNav = $("#tm-main-nav");

            tmMainNav.singlePageNav({
                filter: ':not(.external)'
            });

            $('.navbar-toggler').click(function(e) {
                e.stopPropagation();
                tmMainNav.toggleClass('show');
            });

            $("html").click(function(e) {
                $("#tm-main-nav").removeClass("show");
            });

            /****************** Smooth Scrolling *****************/

            $(".tm-btn-next").on('click', function(event) {
                if (this.hash !== "") {
                    event.preventDefault();
                    var hash = this.hash;

                    $('html, body').animate({
                        scrollTop: $(hash).offset().top
                    }, 800, function(){
                        // window.location.hash = hash;
                    });
                }
            });

            $('.tm-brand-icon').on('click', function(event) {
                $('html, body').animate({
                        scrollTop: $('#intro').offset().top
                    }, 800);
            });

            /****************** Gallery ******************/

            const galleryItems = document.querySelector(".tm-gallery").children;
            const itemsPerPage = 10;
            const totalPages = Math.ceil(galleryItems.length / itemsPerPage);
            const pageAttribute = 'data-page';

            function setPagination(currentPage) {
                for(let i = 1; i <= totalPages; i++) {
                    var $pager = '';
                    
                    if(currentPage == i) {
                        $pager = $('<a href="javascript:void(0);" class="active tm-paging-link" '+pageAttribute+'="'+i+'"></a>');
                    } else {
                        $pager = $('<a href="javascript:void(0);" class="tm-paging-link" '+pageAttribute+'="'+i+'"></a>');
                    }

                    $pager.html(i);

                    $pager.click(function(){ 
                        $('.tm-paging-link').removeClass("active");
                        $(this).addClass('active');
                        var page = $(this).eq(0).attr(pageAttribute);
                        showItems(page);
                    });

                    $pager.appendTo($('.tm-paging'));
                }
            }

            function showItems(currentPage) {
                for(let i = 0; i < galleryItems.length; i++) {
                    galleryItems[i].classList.remove("show");
                    galleryItems[i].classList.add("hide");

                    if(i >= (currentPage * itemsPerPage) - itemsPerPage && i < currentPage * itemsPerPage) {
                        galleryItems[i].classList.remove("hide");
                        galleryItems[i].classList.add("show");
                    }
                }
            }

            setPagination(1);
            showItems(1);

            /****************** Magnific Popup ***********/

            $('.tm-gallery').magnificPopup({
                delegate: 'a',
                type: 'image',
                gallery: {
                    enabled: true
                }
            });
        });
    </script>
</body>
</html>
