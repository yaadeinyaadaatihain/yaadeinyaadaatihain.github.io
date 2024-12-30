# Yaadein Yaad Aati Hain!!!

Yaado Ka kaam hai Yaad Ana.... Dil na lage to Hamari gali aa jana...

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Vertex HTML Template</title>
    <link href="https://fonts.googleapis.com/css2?family=Kumbh+Sans&display=swap" rel="stylesheet">
    <link href="https://fonts.google.com/specimen/Kumbh+Sans" rel="stylesheet">
    <link rel="stylesheet" href="https://fontawesome.com">  
    <link rel="stylesheet" href="https://dimsemenov.com/plugins/magnific-popup">
    <link rel="stylesheet" href="css/tooplate-vertex.css">
<style>
    #loader-wrapper {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    z-index: 1001;
}
#loader {
    display: block;
    position: relative;
    left: 50%;
    top: 50%;
    width: 150px;
    height: 150px;
    margin: -75px 0 0 -75px;
    border-radius: 50%;
    border: 3px solid transparent;
    border-top-color: #3498db;

    -webkit-animation: spin 2s linear infinite; /* Chrome, Opera 15+, Safari 5+ */
    animation: spin 2s linear infinite; /* Chrome, Firefox 16+, IE 10+, Opera */

    z-index: 1002;
}

    #loader:before {
        content: "";
        position: absolute;
        top: 5px;
        left: 5px;
        right: 5px;
        bottom: 5px;
        border-radius: 50%;
        border: 3px solid transparent;
        border-top-color: #e74c3c;

        -webkit-animation: spin 3s linear infinite; /* Chrome, Opera 15+, Safari 5+ */
        animation: spin 3s linear infinite; /* Chrome, Firefox 16+, IE 10+, Opera */
    }

    #loader:after {
        content: "";
        position: absolute;
        top: 15px;
        left: 15px;
        right: 15px;
        bottom: 15px;
        border-radius: 50%;
        border: 3px solid transparent;
        border-top-color: #f9c922;

        -webkit-animation: spin 1.5s linear infinite; /* Chrome, Opera 15+, Safari 5+ */
          animation: spin 1.5s linear infinite; /* Chrome, Firefox 16+, IE 10+, Opera */
    }

    @-webkit-keyframes spin {
        0%   { 
            -webkit-transform: rotate(0deg);  /* Chrome, Opera 15+, Safari 3.1+ */
            -ms-transform: rotate(0deg);  /* IE 9 */
            transform: rotate(0deg);  /* Firefox 16+, IE 10+, Opera */
        }
        100% {
            -webkit-transform: rotate(360deg);  /* Chrome, Opera 15+, Safari 3.1+ */
            -ms-transform: rotate(360deg);  /* IE 9 */
            transform: rotate(360deg);  /* Firefox 16+, IE 10+, Opera */
        }
    }
    @keyframes spin {
        0%   { 
            -webkit-transform: rotate(0deg);  /* Chrome, Opera 15+, Safari 3.1+ */
            -ms-transform: rotate(0deg);  /* IE 9 */
            transform: rotate(0deg);  /* Firefox 16+, IE 10+, Opera */
        }
        100% {
            -webkit-transform: rotate(360deg);  /* Chrome, Opera 15+, Safari 3.1+ */
            -ms-transform: rotate(360deg);  /* IE 9 */
            transform: rotate(360deg);  /* Firefox 16+, IE 10+, Opera */
        }
    }

    #loader-wrapper .loader-section {
        position: fixed;
        top: 0;
        width: 51%;
        height: 100%;
        background: #222222;
        z-index: 1001;
        -webkit-transform: translateX(0);  /* Chrome, Opera 15+, Safari 3.1+ */
        -ms-transform: translateX(0);  /* IE 9 */
        transform: translateX(0);  /* Firefox 16+, IE 10+, Opera */
    }

    #loader-wrapper .loader-section.section-left {
        left: 0;
    }

    #loader-wrapper .loader-section.section-right {
        right: 0;
    }

    /* Loaded */
    .loaded #loader-wrapper .loader-section.section-left {
        -webkit-transform: translateX(-100%);  /* Chrome, Opera 15+, Safari 3.1+ */
            -ms-transform: translateX(-100%);  /* IE 9 */
                transform: translateX(-100%);  /* Firefox 16+, IE 10+, Opera */

        -webkit-transition: all 0.7s 0.3s cubic-bezier(0.645, 0.045, 0.355, 1.000);  
                transition: all 0.7s 0.3s cubic-bezier(0.645, 0.045, 0.355, 1.000);
    }

    .loaded #loader-wrapper .loader-section.section-right {
        -webkit-transform: translateX(100%);  /* Chrome, Opera 15+, Safari 3.1+ */
            -ms-transform: translateX(100%);  /* IE 9 */
                transform: translateX(100%);  /* Firefox 16+, IE 10+, Opera */

-webkit-transition: all 0.7s 0.3s cubic-bezier(0.645, 0.045, 0.355, 1.000);  
        transition: all 0.7s 0.3s cubic-bezier(0.645, 0.045, 0.355, 1.000);
    }
    
    .loaded #loader {
        opacity: 0;
        -webkit-transition: all 0.3s ease-out;  
                transition: all 0.3s ease-out;
    }
    .loaded #loader-wrapper {
        visibility: hidden;

        -webkit-transform: translateY(-100%);  /* Chrome, Opera 15+, Safari 3.1+ */
            -ms-transform: translateY(-100%);  /* IE 9 */
                transform: translateY(-100%);  /* Firefox 16+, IE 10+, Opera */

        -webkit-transition: all 0.3s 1s ease-out;  
                transition: all 0.3s 1s ease-out;
    }

/* General */

* {  box-sizing: border-box; }
html, body { overflow-x: hidden; }
body { 
    font-family: 'Kumbh Sans', sans-serif;
    font-size: 18px;
    background-color: #333;
    color: #999;
    margin: 0;
}
a { color: #fff; text-decoration: none; }
a:hover {  color: #9C9; }
button { cursor: pointer; }
a, button { transition: all 0.3s ease; }
ul {
    margin: 0;
    padding: 0;
}

h2 {
    line-height: 1.6;
    margin-top: 0;
    margin-bottom: 30px;
}

p {
    line-height: 1.8;
    margin-bottom: 50px;
}

span, footer {  line-height: 1.8; }

.tm-btn {
    display: inline-block;
    border: 1px solid #666;
    background-color: transparent;
    color: #999;
    padding: 14px 40px;
    font-size: 20px;
}

.tm-btn:hover {
    color: #99CC99;
    border-color: #99CC99;
}

.tm-text-small { font-size: 0.9em; }
.tm-text-center { text-align: center; }
.tm-text-right { text-align: right; }
.tm-text-primary { color: #99CC99; }
.tm-text-secondary { color: #9999CC; }
.tm-text-link { color: #999; }
.tm-text-link:hover { color: #99CC99; }
.tm-relative { position: relative; }

.tm-hr {
    border-color: #555;
    max-width: 340px;
    width: 100%;    
}

.tm-mr {
    margin-right: 0;
    margin-left: auto;
}

.tm-ml {
    margin-left: 0;
    margin-right: auto;
}

.tm-my-50 {
    margin-top: 50px;
    margin-bottom: 50px;
}
.tm-mb-20 { margin-bottom: 20px; }
.tm-mb-50 { margin-bottom: 50px; }
.tm-mb-80 { margin-bottom: 80px; }
.tm-mb-130 { margin-bottom: 130px; }
.tm-mb-200 { margin-bottom: 200px; }

/* Layout */
.tm-section { display: flex; }

.tm-section-col {
    flex: 0 0 50%;
    width: 50%;
}

.tm-content {
    padding: 180px 60px 70px 100px;
    box-sizing: border-box;
}

.tm-content-small { padding: 190px 120px 70px; }
.tm-content-small-top { padding-top: 130px; }

.tm-row {
    display: flex;
    margin-left: -25px;
    margin-left: -25px;
}

.tm-col {
    flex: 0 0 50%;
    width: 50%;
    padding: 25px;
    box-sizing: border-box;
}

/* Brand */
.tm-brand {
    position: fixed;
    bottom: 80px;
    right: 70px;
    width: 300px;
    height: 240px;
    margin-top: 0;
    margin-bottom: 0;
    background-color: #333;
    color: #999;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
}

.tm-brand-icon { margin-bottom: 25px; }
.tm-brand-text { font-size: 32px; }

/* Nav */
.navbar-toggler { display: none; }

.tm-nav {
    position: fixed;
    top: 0;
    left: -1px;
    width: 50%;
    z-index: 1000;  
}

.tm-nav ul {
    background-color: #444;
    display: flex;
    justify-content: space-around;
}

.nav-item { list-style: none; }

.nav-link {
    color: #999;
    padding-top: 40px;
    padding-bottom: 40px;
    display: block;
    font-size: 20px;
}

.nav-link:hover,
.nav-link.current {
    color: #99CC99;
}

/* Introduction */
.tm-media {
    display: flex;
    align-items: flex-start;
    margin-bottom: 70px;
}

.tm-media img {
    width: 200px;
    height: 200px;
}

.tm-media-body {  padding-left: 30px; }

.tm-media-span {
    margin-bottom: 15px;
    display: block;
    text-align: right;
}

/* Gallery */

.tm-gallery-container {
    max-width: 1400px;
    margin-left: auto;
    margin-right: auto;
}

.tm-gallery-header {
    margin-left: 15px;
    margin-right: 15px;
}

.tm-gallery {
	position: relative;
	list-style: none;
	text-align: center;
    overflow: hidden;
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
}

.tm-gallery figure {
	position: relative;
	z-index: 50;
	/* float: left; */
	overflow: hidden;
	margin: 15px;
	min-width: 200px;
	max-width: 250px;
	max-height: 250px;
	width: 25%;
	text-align: center;
	cursor: pointer;
}

.tm-gallery figure img {
	position: relative;
	display: block;
	min-height: 100%;
	max-width: 100%;
	opacity: 0.8;
}

.tm-gallery figure figcaption {
	padding: 1em;
	color: #fff;
	text-transform: uppercase;
	font-size: 1em;
	-webkit-backface-visibility: hidden;
	backface-visibility: hidden;
}

.tm-gallery figure figcaption::before,
.tm-gallery figure figcaption::after {
	pointer-events: none;
}

.tm-gallery figure figcaption,
.tm-gallery figure figcaption > a {
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
    height: 100%;
    box-sizing: border-box;
}

/* Anchor will cover the whole item by default */
/* For some effects it will show as a button */
.tm-gallery figure figcaption > a {
	z-index: 1000;
	text-indent: 200%;
	white-space: nowrap;
	font-size: 0;
	opacity: 0;
}

.tm-gallery figure h2 {
	word-spacing: -0.15em;
	font-weight: 300;
}

.tm-gallery figure h2 span { font-weight: 800; }

.tm-gallery figure h2,
.tm-gallery figure p {
	margin: 0;
}

.tm-gallery figure p {
	letter-spacing: 1px;
	font-size: 68.5%;
}

/*-----------------*/
/***** Goliath *****/
/*-----------------*/

figure.effect-goliath {
	background: #99cc99;
}

figure.effect-goliath img,
figure.effect-goliath h2 {
	-webkit-transition: -webkit-transform 0.35s;
	transition: transform 0.35s;
}

figure.effect-goliath img {
	-webkit-backface-visibility: hidden;
	backface-visibility: hidden;
}

figure.effect-goliath h2,
figure.effect-goliath p {
	position: absolute;
	bottom: 0;
	left: 0;
    padding: 30px 10px;
    text-align: center;
    width: 100%;
}

figure.effect-goliath p {
	text-transform: none;
	font-size: 90%;
	opacity: 0;
	-webkit-transition: opacity 0.35s, -webkit-transform 0.35s;
	transition: opacity 0.35s, transform 0.35s;
	-webkit-transform: translate3d(0,50px,0);
	transform: translate3d(0,50px,0);
}

figure.effect-goliath:hover img {
	-webkit-transform: translate3d(0,-80px,0);
	transform: translate3d(0,-80px,0);
}

figure.effect-goliath:hover h2 {
	-webkit-transform: translate3d(0,-100px,0);
	transform: translate3d(0,-100px,0);
}

figure.effect-goliath:hover p {
	opacity: 1;
	-webkit-transform: translate3d(0,0,0);
	transform: translate3d(0,0,0);
}

.tm-gallery .tm-gallery-item.hide{ display: none; }

.tm-gallery .tm-gallery-item.show{
	display: block;
	animation: show .5s ease;
}

.tm-paging {
    display: flex;
    justify-content: center;
}

.tm-paging-link {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 50px;
    height: 50px;
    color: #999;
    background-color: #222;
    margin: 7.5px;
}

.tm-paging-link:hover,
.tm-paging-link.active {
    background-color: #444444;
}

@keyframes show {
    0% {
    	opacity: 0;
    	transform: scale(0.9);
    }
    100% {
    	opacity: 1;
    	transform: scale(1);
    }
}

/* Contact */
.tm-contact-form {
    max-width: 400px;
    margin-left: auto;
    margin-right: auto;
}
.form-group { margin-bottom: 40px; }

.form-control {
    color: #999;
    font-size: 20px;
    font-family: 'Kumbh Sans', sans-serif;
    padding: 25px 0;
    width: 100%;
    border: none;
    border-bottom: 1px solid #666;
    background: transparent;
}

.form-control:focus {
    color: #999;
    background: transparent;
}

.mapouter {
    position: absolute;
    top: 240px;
    left: 0;
}

.gmap-canvas { width: 340px; }

.tm-copyright {
    margin-left: -50px;
    margin-bottom: -50px;
}

@media (max-width: 1200px) {
    .tm-nav { width: 0; }
    .tm-nav ul {
        position: relative;
        left: -280px;
        flex-direction: column;
        padding-top: 15px;
        padding-bottom: 15px;        
        width: 280px;
        transition: all 0.5s ease;
    }

    .tm-nav ul.show { left: 0; }

    .nav-link {
        text-align: center;
        padding-top: 20px;
        padding-bottom: 20px;
    }

    .navbar-toggler {
        display: block;
        width: 50px;
        height: 45px;
        font-size: 1.2rem;
        background-color: #444444;
        border: none;
        color: #999999;
        outline: none;
    }

    .navbar-toggler:hover { color: #99CC99; }

    .tm-content {
        padding-left: 20px;
        padding-right: 20px;
        padding: 50px 20px;
    }

    .tm-copyright { margin-left: 15px; }
}

@media (max-width: 992px) {
    .tm-brand { 
        position: static;
        margin-left: auto;
        margin-right: 0;
    }

    .tm-gallery figure { width: 33.33%; }

    figcaption h2 { font-size: 1.4rem; }

    .tm-section { flex-direction: column-reverse; }

    .tm-section-col {
        flex: 0 0 100%;
        width: 100%;
    }

    .tm-parallax { min-height: 360px; }

    #contact .tm-parallax {
        margin-bottom: 425px;
    }
    
    .mapouter {
        top: 360px;
        width: 100%;
    }

    .gmap-canvas { width: 100%; }

    .tm-copyright {
        margin-bottom: 0;
        padding: 30px;
    }
}

@media (max-width: 600px) {
    .tm-row { flex-direction: column; }

    .tm-col {
        flex: 0 0 100%;
        width: 100%;
    }

    .tm-media img {
        width: 150px;
        height: 150px;
    }
}

@media (max-width: 560px) {
    .tm-sm-mt-30 { margin-top: 30px; }
}

@media (max-width: 516px) {
    .tm-gallery { display: block; }

    .tm-gallery figure {
        float: left;
        width: 45%;
        margin: 2.5%;
        min-width: 1px;
    }

    figure h2 { font-size: 1rem; }
}

@media (max-width: 420px) {
    .tm-media img {
        width: 100px;
        height: 100px;
    }
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
        <i class="fas fa-mountain fa-2x tm-brand-icon"></i>
        <span class="tm-brand-text">Vertex</span>        
    </h1>

    <!-- Nav -->
    <nav class="tm-nav">
        <button class="navbar-toggler" type="button" aria-label="Toggle navigation">
            <i class="fas fa-bars"></i>
        </button>
        <ul id="tm-main-nav">
            <li class="nav-item">                                
                <a href="#intro" class="nav-link current">
                    Introduction
                </a>
            </li>
            <li class="nav-item">
                <a href="#services" class="nav-link">
                    Services
                </a>
            </li>
            <li class="nav-item">
                <a href="#gallery" class="nav-link">
                    Gallery
                </a>
            </li>
            <li class="nav-item">
                <a href="#about" class="nav-link">
                    About
                </a>
            </li>
            <li class="nav-item">
                <a href="#contact" class="nav-link">
                    Contact
                </a>
            </li>
        </ul>
    </nav>

    <!-- Content -->
    <main>
        <div id="intro" class="tm-section">
            <!-- Intro left -->
            <div class="tm-section-col tm-content">
                <div class="tm-media">
                    <img src="img/gallery/tn/img-11.jpg" alt="Intro image">
                    <div class="tm-media-body">
                        <h2><a href="#" class="tm-text-primary">Vertex is a Free CSS Template</a></h2>
                        <p class="tm-mb-20 tm-text-small">
                            This is a Responsive HTML5 Template brought to you by Tooplate for
                            100% free of charge. You can feel free to download, modify, and
                            use this layout for your websites.
                        </p>
                        <span class="tm-text-secondary tm-media-span tm-text-small">
                            Friday . 25 June 2021
                        </span>
                        <hr class="tm-hr tm-mr">
                    </div>
                </div>
    
                <div class="tm-media">
                    <img src="img/gallery/tn/img-12.jpg" alt="Intro image">
                    <div class="tm-media-body">
                        <h2><a href="#" class="tm-text-primary">Responsive and Parallax Images</a></h2>
                        <p class="tm-mb-20 tm-text-small">
                      You are not allowed to re-distribute this template as a ZIP file on any template collection website for the template download purpose. Please <a rel="nofollow" href="https://www.tooplate.com/contact" target="_parent">contact us</a> for more info. </p>
                        <span class="tm-text-secondary tm-media-span tm-text-small">
                            Monday . 21 June 2021
                    </span>
                        <hr class="tm-hr tm-mr">
                    </div>
                </div>
                
                <div class="tm-media">
                    <img src="img/gallery/tn/img-18.jpg" alt="Intro image">
                    <div class="tm-media-body">
                        <h2><a href="#" class="tm-text-primary">Do you like this HTML layout?</a></h2>
                        <p class="tm-mb-20 tm-text-small">
                            This is a custom full-width layout. Gallery page included paging thumbnails with a beautiful hover effect and a larger image pop up in the lightbox.
                        </p>
                        <span class="tm-text-secondary tm-media-span tm-text-small">
                            Wednesday . 16 June 2021
                        </span>
                        <hr class="tm-hr tm-mr">
                    </div>
                </div>
                <div class="tm-text-right">
                    <a href="#services" class="tm-btn tm-btn-next">Next page</a>
                </div>   
                
            </div>
            
            <!-- Intro right -->
            <div class="tm-section-col tm-parallax" data-parallax="scroll" data-image-src="img/vertex-bg-01.jpg"></div>
        </div> <!-- #intro -->

        <div id="services" class="tm-section">
            <!-- Services left -->
            <div class="tm-section-col tm-content">
                <h2 class="tm-text-primary">Our Services</h2>
                <p>Credit goes to <strong>Pexels website</strong> for background images and Unsplash website for gallery images used in this Vertex HTML template. Vestibulum quis ultrices ipsum, tempor cursus odio. Donec et nisl sit amet mauris consequat sodales. 
                </p>
                <p>
                    Morbi a sapien vitae nunc mollis efficitur quis eu purus. Donec nec orci pharetra, ullamcorper orci eu, gravida dolor. Morbi at rutrum nibh. Sed a erat vitae ipsum mollis tincidunt sed nec orci.
                </p>
                <div class="tm-text-right">
                    <a href="#gallery" class="tm-btn tm-btn-next">Next page</a>
                </div>                
                <hr class="tm-hr tm-ml tm-sm-mt-30">
                <div class="tm-row">
                    <div class="tm-col">
                        <div class="tm-text-center tm-my-50">
                            <i class="fas fa-street-view fa-3x"></i>
                        </div>                        
                        <p>
                            Fusce mi sapien, faucibus ut tortor a, tempus laoreet magna. Nulla felis ipsum, lobortis eu efficitur eget, malesuada id lacus.
                        </p>
                    </div>
                    <div class="tm-col">
                        <div class="tm-text-center tm-my-50">
                            <i class="fas fa-bullseye fa-3x"></i>
                        </div>                        
                        <p>
                            Nullam pellentesque accumsan hendrerit. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos.
                        </p>
                    </div>
                </div>                
            </div>
            
            <!-- Services right -->
            <div class="tm-section-col tm-parallax" data-parallax="scroll" data-image-src="img/vertex-bg-02.jpg"></div>
        </div> <!-- #services -->

        <div id="gallery" class="tm-content tm-content-small-top">
            <div class="tm-gallery-container">
                <h2 class="tm-text-primary tm-text-right tm-gallery-header">Our Gallery</h2> 
                <div class="tm-gallery tm-mb-80">
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-01.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number One</h2>
                            <p>Best Template Site</p>
                            <a href="img/gallery/img-01.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-02.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 2</h2>
                            <p>Tooplate HTML CSS</p>
                            <a href="img/gallery/img-02.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-03.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 3</h2>
                            <p>Free Template</p>
                            <a href="img/gallery/img-03.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-04.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 4</h2>
                            <p>Free Download</p>
                            <a href="img/gallery/img-04.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-05.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 5</h2>
                            <p>Mobile Ready</p>
                            <a href="img/gallery/img-05.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-06.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 6</h2>
                            <p>Responsive Design</p>
                            <a href="img/gallery/img-06.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-07.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 7</h2>
                            <p>Custom HTML CSS</p>
                            <a href="img/gallery/img-07.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-08.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 8</h2>
                            <p>Template for you</p>
                            <a href="img/gallery/img-08.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-09.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 9</h2>
                            <p>Get it FREE</p>
                            <a href="img/gallery/img-09.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-10.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 10</h2>
                            <p>Tell your friends</p>
                            <a href="img/gallery/img-10.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-11.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Picture 11</h2>
                            <p>Aliquam lacinia</p>
                            <a href="img/gallery/img-11.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-12.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Item 12</h2>
                            <p>Aliquam lacinia</p>
                            <a href="img/gallery/img-12.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-13.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 13</h2>
                            <p>Aliquam lacinia</p>
                            <a href="img/gallery/img-13.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-14.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Picture 14</h2>
                            <p>Aliquam lacinia</p>
                            <a href="img/gallery/img-14.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-15.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Pic 15</h2>
                            <p>Aliquam lacinia</p>
                            <a href="img/gallery/img-15.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-16.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Pic 16</h2>
                            <p>Aliquam lacinia</p>
                            <a href="img/gallery/img-16.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-17.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 17</h2>
                            <p>Aliquam lacinia</p>
                            <a href="img/gallery/img-17.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-18.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Pic 18</h2>
                            <p>Aliquam lacinia</p>
                            <a href="img/gallery/img-18.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-19.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Pic 19</h2>
                            <p>Aliquam lacinia</p>
                            <a href="img/gallery/img-19.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-20.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 20</h2>
                            <p>Aliquam lacinia</p>
                            <a href="img/gallery/img-20.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-21.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Pic 21</h2>
                            <p>Aliquam lacinia</p>
                            <a href="img/gallery/img-21.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-22.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Pic 22</h2>
                            <p>Aliquam lacinia</p>
                            <a href="img/gallery/img-22.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-23.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Pic 23</h2>
                            <p>Aliquam lacinia</p>
                            <a href="img/gallery/img-23.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-24.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 24</h2>
                            <p>Web Design 2021</p>
                            <a href="img/gallery/img-24.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-25.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 25</h2>
                            <p>Website Design</p>
                            <a href="img/gallery/img-25.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-05.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 26</h2>
                            <p>HTML CSS Layout</p>
                            <a href="img/gallery/img-05.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-04.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 27</h2>
                            <p>Aliquam lacinia</p>
                            <a href="img/gallery/img-04.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-03.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 28</h2>
                            <p>Aliquam lacinia</p>
                            <a href="img/gallery/img-03.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-02.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 29</h2>
                            <p>Aliquam lacinia</p>
                            <a href="img/gallery/img-02.jpg">View more</a>
                        </figcaption>			
                    </figure>
                    <figure class="effect-goliath tm-gallery-item">
                        <img src="img/gallery/tn/img-01.jpg" alt="Image"/>
                        <figcaption>
                            <h2>Number 30</h2>
                            <p>Aliquam lacinia</p>
                            <a href="img/gallery/img-01.jpg">View more</a>
                        </figcaption>			
                    </figure>
                </div>
                <div class="tm-paging tm-mb-130"></div>
            </div>
        </div>

        <div id="about" class="tm-section">
            <!-- About left -->
            <div class="tm-section-col tm-content tm-content-small">
                <h2 class="tm-text-primary">About Us</h2>
                <p>
                    You can find more free templates on Too CSS collections. Please visit Too CSS website to see a great list of HTML CSS templates. Simply type it in Google search.
                </p>
                <p>
                    You may help us by spreading a word about our website or make a small contribution by contacting Tooplate directly. That will be very helpful for us. Thank you.
                </p>
                <hr class="tm-hr tm-mb-50">                
                <p class="tm-mb-50">
                    Quisque luctus feugiat dui eget malesuada. Donec rutrum, nibh vel lobortis placerat, leo enim feugiat arcu, ornare imperdiet urna sem vitae tellus.
                </p>
                <div class="tm-text-right tm-mb-130">
                    <a href="#contact" class="tm-btn tm-btn-next">Contact Us</a>
                </div>                
            </div>
            
            <!-- About right -->
            <div class="tm-section-col tm-parallax" data-parallax="scroll" data-image-src="img/vertex-bg-03.jpg"></div>
        </div> <!-- #about -->

        <div id="contact" class="tm-section">
            <!-- Contact left -->
            <div class="tm-section-col tm-content tm-content-small">
                <h2 class="tm-text-primary">Contact Us</h2>
                <p>
                    Pellentesque nec dui pellentesque, fermentum turpis eu, facilisis libero. Vestibulum fringilla nulla augue, at consequat metus facilisis condimentum.
                </p> 
                <form id="contact-form" action="" method="POST" class="tm-contact-form tm-mb-200">
                    <div class="form-group">
                        <input type="text" name="name" class="form-control rounded-0" placeholder="Name" required />
                    </div>
                    <div class="form-group">
                        <input type="email" name="email" class="form-control rounded-0" placeholder="Email" required />
                    </div>
                    <div class="form-group">
                        <textarea rows="6" name="message" class="form-control rounded-0" placeholder="Message" required=></textarea>
                    </div>

                    <div class="form-group tm-text-right">
                        <button type="submit" class="tm-btn">Send</button>
                    </div>
                </form>
                <footer class="tm-copyright tm-text-small">
                    Copyright 2021 Vertex Company 
                    
                    - Design: <a rel="nofollow" href="https://www.tooplate.com" class="tm-text-link" target="_parent">Tooplate</a>
                </footer>              
            </div>
            
            <!-- Contact right -->
            <div class="tm-section-col tm-parallax tm-relative" data-parallax="scroll" data-image-src="img/vertex-bg-04.jpg">
                <!-- Map -->
                <div class="mapouter">
                    <div class="gmap-canvas">
                        <iframe width="100%" height="420" id="gmap_canvas"
                            src="https://maps.google.com/maps?q=Av.+L%C3%BAcio+Costa,+Rio+de+Janeiro+-+RJ,+Brazil&t=&z=13&ie=UTF8&iwloc=&output=embed"
                            frameborder="0" scrolling="no" marginheight="0" marginwidth="0"></iframe>
                    </div>
                </div>
            </div>
        </div> <!-- #contact -->
    </main>

<!-- JS -->

</body>
</html>
