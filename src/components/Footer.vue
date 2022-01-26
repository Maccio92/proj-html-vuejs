<template>
<footer>
    <div class="footer container-fluid d-flex align-items-center justify-content-center py-5">
        <div class="row row-cols-12 justify-content-center">
            <div class="col-2">
                <h2 class="data-light">About</h2>
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
                <h2 class="data-light">Twitter</h2>
                <div class="line my-4"></div>
                <div class="d-flex align-items-start ">
                    <i class="fab fa-twitter text-orange me-1"></i>
                    <p class="features-caption">Lorem ipsum dolor sit amet consectetur adipisicing elit. In fugiat commodi eveniet, est debitis nesciunt non blanditiis ducimus iusto.</p>  
                </div>
                <div class="d-flex">
                    <i class=" fab fa-twitter text-orange me-1"></i>
                    <p class="features-caption">orem ipsum dolor sit amet consectetur adipisicing elit. In fugiat commodi eveniet, est debitis nesciunt non blanditiis ducimus iusto.</p>  
                </div>
            </div>
            <div class="col-2">
                <h2 class="data-light">Important Links</h2>
                <div class="line my-4"></div>
                <ul class="list-unstyled">
                    <li><a class="text-decoration-none features-caption" href="#">About me</a>  </li>
                    <li><a class="text-decoration-none features-caption" href="#">About us</a>  </li>
                    <li><a class="text-decoration-none features-caption" href="#">Language packs</a>  </li>
                    <li><a class="text-decoration-none features-caption" href="#">Become a coach</a>  </li>
                    <li><a class="text-decoration-none features-caption" href="#">Monthly events</a>  </li>
                </ul> 
            </div>
            <div class="col-2">
                <h2 class="data-light">Contact Me</h2>
                <div class="line my-4"></div>
                <div class="d-flex align-items-center">
                    <i class="far fa-clock text-orange"></i>
                    <p class="my-2 ps-2 features-caption">457 BigBlue Street, NY 10013</p>
                </div>
                <div class="d-flex align-items-center">
                    <i class="fas fa-phone-alt text-orange"></i>
                    <p class="my-2 ps-2 features-caption">(315)5512-2579</p>
                </div>
                <div class="d-flex align-items-center mb-2 ">
                    <i class="fas fa-map-marker-alt text-orange"></i>
                    <p class="my-2 ps-2 features-caption-">everlead@mikado.com</p>
                </div> 
                <div class="d-flex border-bottom align-items-center">
                    <input type="text" class="form-control border-0 bg-transparent me-2" placeholder="Your Name" aria-label="Username" aria-describedby="basic-addon1">
                    <a class="text-light text-decoration-none pt-1" href="#">SUBSCRIBE</a>
                </div>
                
            </div>
        </div>
        
    </div>
    <div class="end-bar">
        <p class="text-light copy">Copyright Everlead@Mikadothemes</p>
    </div>
</footer>
</template>

<script>
export default {
name: 'Footer',
}
</script>

<style lang="scss" scoped>
.footer{
    background-color: #191516 ;
}
.end-bar{
        height: 20px;
        background-color: #ff4612;
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
.copy{
    text-align: center;
    font-size: 0.5em;
}
</style>