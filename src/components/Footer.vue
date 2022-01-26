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
                    <FooterMenu 
                    v-for="(item,index) in footerMenu"
                    :key="index"
                    :link="item.href"
                    :name="item.name"
                    />
                </ul> 
            </div>
            <FooterContact
            v-for="(contact,index) in footerContact"
            :key="index"
            :menuTitle="contact.title"
            :location="contact.location"
            :phone="contact.number"
            :mail="contact.mail"
            />
        </div>
        
    </div>
    <div class="end-bar">
        <p class="text-light copy">Copyright Everlead@Mikadothemes</p>
    </div>
</footer>
</template>

<script>
import FooterMenu from './FooterMenu.vue';
import FooterContact from './FooterContact.vue';

export default {
name: 'Footer',
components:{
    FooterContact,
    FooterMenu,
    },
    data(){
        return{
            footerContact:[
                {
                    title:'Contact Me',
                    location: '457 BigBlue Street, NY 10013',
                    number: '(315)5512-2579',
                    mail:'everlead@mikado.com'
                }

            ],
            footerMenu: [
                {
                    href: "#",
                    name: "About Me",
                },
                {
                    href: "#",
                    name: "About us",
                },
                {
                    href: "#",
                    name: "Language packs",
                },
                {
                    href: "#",
                    name: "Become a coach",
                },
                {
                    href: "#",
                    name: "Monthly events",
                },
            ]
        }
    }
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
.line{
    margin: 0;
}
</style>