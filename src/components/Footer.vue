<template>
<footer>
    <div class="footer container-fluid d-flex align-items-center justify-content-center py-5">
        <div class="row row-cols-12 justify-content-center">
            <div class="col-2">
                <h2 class="footer-title">About</h2>
                <div class="line my-4"></div>
                <p class="features-caption">Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
                <div class="d-flex gap-3 my-4">
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
            <div class="col-2">
                <h2 class="footer-title">Twitter</h2>
                <div class="line my-4"></div>
                <div class="d-flex align-items-start ">
                    <i class="fab fa-twitter orange me-1"></i>
                    <p class="footer-text">Lorem ipsum dolor sit amet consectetur adipisicing elit. In fugiat commodi eveniet, est debitis nesciunt non blanditiis ducimus iusto.</p>  
                </div>
                <div class="d-flex">
                    <i class=" fab fa-twitter orange me-1"></i>
                    <p class="footer-text">orem ipsum dolor sit amet consectetur adipisicing elit. In fugiat commodi eveniet, est debitis nesciunt non blanditiis ducimus iusto.</p>  
                </div>
            </div>
            <div class="col-2">
                <h2 class="footer-title">Important Links</h2>
                <div class="line my-4"></div>
                <ul class="list-unstyled">
                    <li><a class="text-decoration-none footer-text" href="#">About me</a>  </li>
                    <li><a class="text-decoration-none footer-text" href="#">About us</a>  </li>
                    <li><a class="text-decoration-none footer-text" href="#">Language packs</a>  </li>
                    <li><a class="text-decoration-none footer-text" href="#">Become a coach</a>  </li>
                    <li><a class="text-decoration-none footer-text" href="#">Monthly events</a>  </li>
                </ul> 
            </div>
            <div class="col-2">
                <h2 class="footer-title">Contact Me</h2>
                <div class="line my-4"></div>
                <div class="d-flex align-items-center">
                    <i class="far fa-clock orange"></i>
                    <p class="my-2 ps-2 footer-text">457 BigBlue Street, NY 10013</p>
                </div>
                <div class="d-flex align-items-center">
                    <i class="fas fa-phone-alt orange"></i>
                    <p class="my-2 ps-2 footer-text">(315)5512-2579</p>
                </div>
                <div class="d-flex align-items-center mb-2 ">
                    <i class="fas fa-map-marker-alt orange"></i>
                    <p class="my-2 ps-2 footer-text">everlead@mikado.com</p>
                </div> 
            </div>
        </div>
        
    </div>
    <div class="end-bar"></div>
</footer>
</template>

<script>
export default {
name: 'Footer',
}
</script>

<style lang="scss" scoped>
.footer{
    // height: 300px;
    background-color: #191516 ;
}
.end-bar{
        height: 20px;
        background-color: #ff4612;
}
.footer-title{
    color: white;
    font-family: 'Times New Roman', Times, serif;
    font-size: 1em;
}
.line{ 
    width: 20%;
    border-bottom: solid #ff4612 2px;
}
.social{
    background-color: white;
}
.social-icon {
    color: black;
    position: absolute;
    left: 50%;
    top: 50%;
    transform: translate(-50%, -50%);
}
.footer-text{
    font-size: 0.8em;
    font-weight: 300;
    color: #606060;
}
</style>