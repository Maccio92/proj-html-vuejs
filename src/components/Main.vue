<template>
<main>
    <!-- Jumbotron -->
    <div id="carouselExampleCaptions" class="carousel slide" data-bs-interval="false">
        <div class="carousel-indicators">
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active" aria-current="true" aria-label="Slide 1"></button>
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1" aria-label="Slide 2"></button>
        </div>
        <div class="carousel-inner">
            <div class="carousel-item active position-relative">
                <img src="../assets/img/rev-slider-main-home-img-03.jpg" class="d-block w-100" alt="...">
                <div class="carousel-caption d-none d-md-block position-absolute">
                    <h1 class="title text-black mb-5">Our Team<span class="point">.</span></h1>
                    <p class="subtitle mb-5" >Lorem ipsum dolor, sit amet consectetur adipisicing elit,<br>Aperiam aliquam, expedita fuga.</p>
                    <button class="border-0 px-4 py-3 button me-1">
                        Read More
                        <div class="border-button d-inline">
                            <i class=" fas fa-long-arrow-alt-right ms-2"></i>
                        </div>
                        
                    </button>
                    <button class="border-0 px-4 py-3 bg-orange ms-1">
                        Purchase
                        <div class="border-button d-inline">
                            <i class=" fas fa-long-arrow-alt-right ms-2"></i>    
                        </div>
                    </button>
                </div>
            </div>
            <div class="carousel-item">
                <img src="../assets/img/rev-slider-main-home-img-02.png" class="d-block w-100" alt="...">
            </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="prev" data-interval="false">
            <span class="sx-arrow fas fa-long-arrow-alt-left carousel-control-prev-icon" aria-hidden="true"></span>

        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide="next" data-interval="false">
            <span class="dx-arrow fas fa-long-arrow-alt-right carousel-control-next-icon " aria-hidden="true"></span>
        </button>
    </div>
    <!-- Specialità -->
    <div class="container-80 text-center my-5 d-flex flex-column align-items-center">
        <div class="row" >
            <h2 class="section-title m-0">Our specialities<span class="point">.</span></h2>
            <h5 class="subtitle my-2">Lorem ipsum dolor sit amet consectetur adipisicing elit.</h5>
            <div class="line mt-2"></div>
        </div>
    </div>
    <!-- Features -->
    <div class="container-80">
        <ul class="list-unstyled list-inline row justify-content-center gx-3 ">
            <Features 
                v-for="(feature, index) in features"
                :key="index"
                :img="feature.img"
                :title="feature.title"
                :caption="feature.caption"
            />
        </ul>
    </div>  
    <!-- Sezione Founder -->
    <div class="container-80 py-5 bg-image-dx">
        <div class="row align-items-center position-relative ">
            <div class="col-6">
                <img class="image-team" src="../assets/img/h1-img-01.jpg" alt=""> 
            </div>
            <div class="col-5 blank p-5">
                <h2 class="section-title">Jason Bickford</h2>
                <p class="features-caption">Founder and Executive Director </p>
                <div class="line my-4"></div>
                <p class="features-caption">Lorem ipsum dolor sit amet, consectetur adipisicing elit. Exercitationem commodi quam doloremque illum ipsam error, veritatis.</p>
                <div class="d-flex gap-3">
                    <div class="rounded-circle social position-relative">
                        <i class="social-icon fab fa-linkedin-in"></i>
                    </div>
                    <div class="rounded-circle social position-relative">
                        <i class="social-icon fab fa-facebook-f"></i>
                    </div>
                    <div class="rounded-circle social position-relative">
                        <i class="social-icon fab fa-twitter"></i>
                    </div>
                </div>
            </div>
        </div>
    </div>
    <!-- Sezione Eventi -->
    <div class="container-fluid bg-events my-5 position-relative">
            <div class="row centering">
                <div class="container">
                    <div class="bg-light p-5">
                        <h3 class="event-title mb-5">Upcoming Events</h3>
                        <ul class="list-unstyled">
                            <li class="d-flex mb-5 ">
                                <div class="data-container d-flex flex-column justify-content-center align-items-center">
                                    <p class="data">07</p>
                                    <p class="data-light">Jan 2022</p>
                                </div>
                                <div class="ps-3">
                                    <h4 class="features-title">Melbourne Coaching</h4>
                                    <div class="d-flex align-items-center">
                                        <i class="far fa-clock text-orange"></i>
                                    <p class="m-0 ps-2">9:00am - 5:00pm, Jan 7, 2022</p>
                                    </div>
                                    <div class="d-flex align-items-center mb-2 ">
                                        <i class="fas fa-map-marker-alt text-orange"></i>
                                    <p class="m-0 ps-2">Cambridge, MA 02138, USA</p>
                                    </div>
                                    <a class="text-decoration-none text-dark fw-bolder" href="#">Read More</a>
                                </div>
                            </li>
                            <li class="d-flex mb-5">
                                <div class="data-container d-flex flex-column justify-content-center align-items-center">
                                    <p class="data">11</p>
                                    <p class="data-light">Jan 2022</p>
                                </div>
                                <div class="ps-3">
                                    <h4 class="features-title">New York Coaching</h4>
                                    <div class="d-flex align-items-center">
                                        <i class="far fa-clock text-orange"></i>
                                    <p class="m-0 ps-2">9:00am - 5:00pm, Jan 11, 2022</p>
                                    </div>
                                    <div class="d-flex align-items-center mb-2 ">
                                        <i class="fas fa-map-marker-alt text-orange"></i>
                                    <p class="m-0 ps-2">Cambridge, MA 02138, USA</p>
                                    </div>
                                    <a class="text-decoration-none text-dark fw-bolder" href="#">Read More</a>
                                </div>
                            </li>
                            <li class="d-flex mb-5">
                                <div class="data-container d-flex flex-column justify-content-center align-items-center">
                                    <p class="data">21</p>
                                    <p  class="data-light">Jan 2022</p>
                                </div>
                                <div class="ps-3">
                                    <h4 class="features-title">London Coaching</h4>
                                    <div class="d-flex align-items-center">
                                        <i class="far fa-clock text-orange"></i>
                                    <p class="m-0 ps-2">9:00am - 5:00pm, Jan 21, 2022</p>
                                    </div>
                                    <div class="d-flex align-items-center mb-2 ">
                                        <i class="text-orange fas fa-map-marker-alt "></i>
                                    <p class="m-0 ps-2">Cambridge, MA 02138, USA</p>
                                    </div>
                                    <a class="text-decoration-none text-dark fw-bolder" href="#">Read More</a>
                                </div>
                                
                            </li>
                        </ul>
                    </div>
                </div>
                
            </div>
    </div>
    <!-- Sezione Creative -->
    <div class="container py-5">
            <div class="row">
                <div class="container-80 d-flex">
                    <div class="col-6 pe-5">
                        <h3 class="event-title">Creative Leader</h3>
                        <div class="line my-3"></div>
                        <p class="features-caption">Lorem ipsum dolor sit amet consectetur adipisicing elit. Sapiente necessitatibus velit amet illum dignissimos sit accusamus, repellat ratione illo vitae quisquam voluptate.</p>
                        <a class="text-decoration-none text-dark fw-bolder" href="#">Read More</a>
                    </div>
                    <div class="col-6 ">
                        <div class="progress-bar-wrapper">
                            <div class="progress-bar-label d-flex justify-content-between">
                                <p>Mentorship</p>
                                <p>78%</p>
                            </div>
                            <div class="height-bar progress">
                                <div class="bg-orange progress-bar" role="progressbar" style="width: 78%" aria-valuenow="50" aria-valuemin="0" aria-valuemax="100"></div>
                            </div>
                            <div class="progress-bar-wrapper">
                                <div class="progress-bar-label d-flex justify-content-between">
                                    <p>Education</p>
                                    <p>95%</p>
                                </div>
                                <div class="height-bar progress">
                                    <div class="bg-orange progress-bar" role="progressbar" style="width: 95%" aria-valuenow="50" aria-valuemin="0" aria-valuemax="100"></div>
                                </div>
                            </div>
                            <div class="progress-bar-wrapper">
                                <div class="progress-bar-label d-flex justify-content-between">
                                    <p>Learning</p>
                                    <p>65%</p>
                                </div>
                                <div class="height-bar progress">
                                    <div class="bg-orange progress-bar" role="progressbar" style="width: 65%" aria-valuenow="50" aria-valuemin="0" aria-valuemax="100"></div>
                                </div>
                            </div>
                            <div class="progress-bar-wrapper">
                                <div class="progress-bar-label d-flex justify-content-between">
                                    <p>Motivation</p>
                                    <p>83%</p>
                                </div>
                                <div class="height-bar progress">
                                    <div class=" bg-orange progress-bar " role="progressbar" style="width: 83%" aria-valuenow="50" aria-valuemin="0" aria-valuemax="100"></div>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
    </div>
    <!-- Sezione News -->
    <div class="container my-5 bg-image-sx">
        <div class="row row-cols-10">
            <div class="container-80 d-flex flex-column align-items-center">
                <h2 class="section-title m-0">Latest News<span class="point">.</span></h2>
                <h5 class="subtitle my-2">Lorem ipsum dolor sit amet consectetur adipisicing elit.</h5>
                <div class="line mt-2"></div>
                <div class="d-flex justify-content-around mt-5 align-items-center">
                    <button class="sx-arrow fas fa-long-arrow-alt-left" type="button"></button>
                    <div class="card col-3 border-0">
                        <div class="crop w-100">
                            <img class="w-100 " src="../assets/img/h1-blog-img-02.jpg" alt="">
                        </div>
                        <div class="crop-down w-100 position-relative ">
                            <img class="w-100 position-absolute bottom-0 start-0" src="../assets/img/h1-blog-img-03.jpg" alt="">
                        </div>
                        <div class="bg-orange position-absolute d-flex align-items-center justify-content-center p-2 orange-label ">
                                <i class="text-light fas fa-tag"></i>
                                <p class="text-light m-0 ps-1">Business, Leading</p>
                        </div>
                        <div class="d-flex align-items-center justify-content-start py-3 ">
                                <i class="far fa-clock text-orange features-caption"></i>
                                <p class="m-0 px-2 features-caption">May 5, 2019 </p>
                                <i class="text-orange far fa-user features-caption"></i>
                                <p class="m-0 ps-2 features-caption">Amanda Doe</p>
                        </div>
                        <h3 class="event-title">Next Investment</h3>
                        <p class="features-caption">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                        <a class="text-decoration-none text-dark fw-bolder" href="#">Read More</a>
                    </div>
                    <div class="card col-3 border-0">
                        <div class="crop w-100">
                            <img class="w-100 " src="../assets/img/h1-blog-img-03.jpg" alt="">
                        </div>
                        <div class="crop-down w-100 position-relative">
                            <img class="w-100 position-absolute bottom-0 start-0" src="../assets/img/h1-blog-img-04.jpg" alt="">
                            </div>
                        <div class="bg-orange position-absolute d-flex align-items-center justify-content-center p-2 orange-label ">
                                <i class="text-light fas fa-tag"></i>
                                <p class="text-light m-0 ps-1">Business, Leading</p>
                        </div>
                        <div class="d-flex align-items-center justify-content-start py-3 ">
                                <i class="far fa-clock text-orange features-caption"></i>
                                <p class="m-0 px-2 features-caption">May 5, 2019 </p>
                                <i class="text-orange far fa-user features-caption"></i>
                                <p class="m-0 ps-2 features-caption">Amanda Doe</p>
                        </div>
                        <h3 class="event-title">Team Building</h3>
                        <p class="features-caption">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                        <a class="text-decoration-none text-dark fw-bolder" href="#">Read More</a>
                    </div>
                    <div class="card col-3 border-0">
                        <div class="crop w-100">
                            <img class="w-100 " src="../assets/img/h1-blog-img-04.jpg" alt="">
                        </div>
                        <div class="crop-down w-100 position-relative">
                            <img class="w-100 position-absolute bottom-0 start-0" src="../assets/img/h1-blog-img-01.jpg" alt="">
                        </div>
                        <div class="bg-orange position-absolute d-flex align-items-center justify-content-center p-2 orange-label ">
                                <i class="text-light fas fa-tag"></i>
                                <p class="text-light m-0 ps-1">Business, Leading</p>
                        </div>
                        <div class="d-flex align-items-center justify-content-start py-3 ">
                                <i class="far fa-clock text-orange features-caption"></i>
                                <p class="m-0 px-2 features-caption">May 5, 2019 </p>
                                <i class="text-orange far fa-user features-caption"></i>
                                <p class="m-0 ps-2 features-caption">Amanda Doe</p>
                        </div>
                        <h3 class="event-title">New Business Day</h3>
                        <p class="features-caption">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                        <a class="text-decoration-none text-dark fw-bolder" href="#">Read More</a>
                    </div>
                    <button class="dx-arrow fas fa-long-arrow-alt-right" type="button"></button>
                </div>
            </div>
        </div>
    </div>
    <!-- Sezione Testimonianze   -->
    <div class="container-fluid bg-dark p-2 bg-opacity-75 height-300 position-relative">
            <p class="testimonial float">Testimonials<span class="point">.</span></p>
            <div class="row">
                <div class=" position-absolute top-50 start-50 translate-middle m-0 w-50 d-flex flex-column align-items-center">
                        <img src="../assets/img/h3-img-04.png" class="d-block w-25 p-5" alt="...">
                        <p class="text-light my-1 testimonial-name ">Cynthia Clark</p>
                        <p class="text-light fw-light" >Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                </div>
            </div>
            <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="prev">
                <a class="fas fa-long-arrow-alt-left"></a>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleIndicators" data-bs-slide="next">
                <a class="fas fa-long-arrow-alt-right" ></a>
            </button>
    </div>
    <!-- Sezione Video -->
    <div class="container-fluid">
            <div class="row">
                <div class="bg-video">
                    <div class="position-absolute svg-icon-1 d-flex align-items-center justify-content-center">
                        <img class="w-50 fill" src="../assets/img/svg-8.svg" alt="">
                    </div>
                    <div  class=" position-absolute svg-icon-2 d-flex align-items-center justify-content-center">
                        <img class="w-50" src="../assets/img/svg-7.svg" alt="">
                    </div>
                
                    <i class="text-light fs-1 fas fa-play position-absolute top-50 start-50 translate-middle"></i>
                </div>
            </div>
    </div>
    <!-- Sezione Contatti -->
    <div class="container-80 my-5 ">
        <div class="row row-cols-12 justify-content-around">
            <div class="col-6 world my-5 position-relative">
                <div class="position-absolute inner-text py-2 px-3">
                    <p class="m-0">New York Coaching</p>
                    <a class="text-decoration-none text-dark fw-bolder" href="#">Read More</a>
                </div>
                <img class="pointer-1 position-absolute" src="../assets/img/h1-contact-rev-02.png" alt="">
                <img class="pointer-2 position-absolute"  src="../assets/img/h1-contact-rev-02.png" alt="">
                <img class="pointer-3 position-absolute"  src="../assets/img/h1-contact-rev-02.png" alt="">
            </div>
            <div class="col-6 my-5">
                <h2 class="section-title mb-3">Contact Us<span class="point">.</span></h2>
                <div class="line my-2"></div>
                <p class="features-caption">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                <div class="my-5">
                    <div class="input-group mb-5">
                        <input type="text" class="form-control border-0" placeholder="Your Name" aria-label="Username" aria-describedby="basic-addon1">
                        <input type="text" class="form-control border-0" placeholder="Your Mail" aria-label="Username" aria-describedby="basic-addon1">
                    </div>
                    <div class="input-group mb-5">
                        <input type="text" class="form-control border-0" placeholder="Write a message" aria-label="Username" aria-describedby="basic-addon1">
                    </div>
                    <button class="border-0 px-4 py-3 bg-orange ms-1 text-light">
                    Purchase
                    <div class="border-button d-inline">
                        <i class=" fas fa-long-arrow-alt-right ms-2"></i>    
                    </div>
                </button>
                </div>
            </div>
        </div>
    </div>
    <!-- Sezione Partner -->
    <div class="container-80">
        <div class="row row-cols-10 justify-content-around">
            <img class="partner-img col-2 p-5" src="../assets/img/h4-clients-img-03.png" alt="">
            <img class="partner-img col-2 p-5" src="../assets/img/h4-clients-img-05.png" alt="">
            <img class="partner-img col-2 p-5" src="../assets/img/h4-clients-img-07.png" alt="">
            <img class="partner-img col-2 p-5" src="../assets/img/h4-clients-img-09.png" alt="">
            <img class="partner-img col-2 p-5" src="../assets/img/h4-clients-img-01.png" alt="">
        </div>
    </div>
</main>
</template>

<script>
import Features from './Features.vue';
export default {
name: 'Main',
components:{
    Features,
},
data(){
    return{
        features:[
            {
                img: require('../assets/img/svg-0.svg'),
                title: 'Knowing',
                caption: 'Lorem ipsum dolor sit amet consectetur adipisicing elit.',
            },
            {
                img: require('../assets/img/svg-1.svg'),
                title: 'Selling',
                caption: 'Lorem ipsum dolor sit amet consectetur adipisicing elit.',
            },
            {
                img: require('../assets/img/svg-2.svg'),
                title: 'Learning',
                caption: 'Lorem ipsum dolor sit amet consectetur adipisicing elit.',
            },
            {
                img: require('../assets/img/svg-3.svg'),
                title: 'Contact',
                caption: 'Lorem ipsum dolor sit amet consectetur adipisicing elit.',
            }

        ]
    }
}
}
</script>

<style lang="scss">
/* Testi */
.title{
    font-size: 4em;
    font-family: 'Times New Roman', Times, serif;
    font-weight: 700;
}
.subtitle{
    color: #555555 ;
    font-size: 0.9em;
    font-weight: 300;
}
.team{
    font-size: 2.5em;
    color: black;
    font-family: 'Times New Roman', Times, serif;
    font-weight: 700;
}
.event-title{
    font-size: 1.7em;
    color: black;
    font-family: 'Times New Roman', Times, serif;
    font-weight: 700;
}
.testimonial{
    text-align: center;
    font-size: 10em;
    font-family: 'Times New Roman', Times, serif;
}
.testimonial-name{
    font-family: 'Times New Roman', Times, serif;
    font-size: 1.4em;
}
/* Carosello */
.dx-arrow, .sx-arrow{
    color: black;
    font-size: 2em;
}
.carousel-control-next-icon, .carousel-control-prev-icon{
    background-image: none !important;
}
.carousel-caption{
    top: 35%;
    left: -40%;
    transform: translate(-30%);
}

/* Pulsanti */
.border-button{
    border-left: solid black 1px;
}
.button{
    background-color: #e1e1e1;
}
.button:hover, .bg-orange:hover{
    cursor: pointer;
    background-color: #ff4612;
    color: white;   
    border-left: solid white 1px;
}
/* Img */
.image-team{
    width: 100%;
}
.bg-image-dx{
    background-repeat: no-repeat;
    background-position-x: 100%;
    background-position-y: 5%;
    background-image: url("../assets/img/svg-4.svg");
}
.bg-image-sx{
    background-repeat: no-repeat;
    background-position-x: 0;
    background-position-y: 0;
    background-image: url("../assets/img/svg-4.svg");
    background-size: cover;
}
.bg-events{
    height: 1000px;
    background-image: url("../assets/img/h1-img-09.jpg");
}
.bg-video{
    height: 700px;
    background-image: url("../assets/img/h1-img-04.jpg");
    background-size: cover;
    background-repeat: no-repeat;
    background-position: center;
    position: relative;
}
.crop{
    height: 80px;
    overflow: hidden;
}
.crop-down{
    height: 140px;
    overflow: hidden;
}

/* Icone */
.social{
    width: 30px;
    height: 30px;
    background-color: #ff4612;
}
.social-icon {
    color: white;
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
}
.social:hover{
background-color: black;
cursor: pointer;
}
.svg-icon-1{
    width: 30px;
    height: 30px;
    color: white;
    background-color: #ee2852;
    top: 0;
    right:0;
}
.svg-icon-2{
    width: 30px;
    height: 30px;
    background-color: white;
    top: 40px;
    right:0; 
}

/* Contact item */
.world{
    background-image: url("../assets/img/h1-contact-rev-01.png");
    background-size: 80%;
    background-position: center;
    background-repeat: no-repeat;
}
.pointer-1{
    width: 3%;
    top: 45%;
    left: 30%;
}
.pointer-2{
    width: 3%;
    top: 35%;
    left: 50%;
}
.pointer-3{
    width: 3%;
    bottom: 32%;
    right: 22%;
}
// Linea Arancione
.line{ 
    width: 10%!important;
    margin: 0 auto;
    border-bottom: solid #ff4612 2px;
}


.blank{
    height: 80%;
    background-color: white;
    position: absolute;
    right: 17%;
}
.data-container{
    width: 80px;
    height: 70px;
    background-color: #ff4612;
}
.centering{
    position: absolute;
    top: 50%;
    left: 30%;
    transform: translate(-50%, -50%);
}
.features-title:hover{
    color: #ff4612;
    cursor: pointer;
}
// Barre progressione
.height-bar{
    height: 0.5em!important;
}
.orange-label{
    bottom: 37%;
    right: 5%;
    font-size: 0.7em;
}
.fill{
    fill: white
}
.height-300{
    height: 400px;
}
.inner-text{
    width: 35%;
    height: 15%;
    top: 52%;
    left: 25%;
    background-color: white;
}
</style>