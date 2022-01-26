<template>
<div class="col-2">
                <h2 class="data-light">{{menuTitle}}</h2>
                <div class="line my-4"></div>
                <div class="d-flex align-items-center">
                    <i class="far fa-clock text-orange"></i>
                    <p class="my-2 ps-2 features-caption">{{location}}</p>
                </div>
                <div class="d-flex align-items-center">
                    <i class="fas fa-phone-alt text-orange"></i>
                    <p class="my-2 ps-2 features-caption">{{phone}}</p>
                </div>
                <div class="d-flex align-items-center mb-2 ">
                    <i class="fas fa-map-marker-alt text-orange"></i>
                    <p class="my-2 ps-2 features-caption-">{{mail}}</p>
                </div> 
                <div class="d-flex border-bottom align-items-center">
                    <input type="text" class="form-control border-0 bg-transparent me-2" placeholder="Your Name" aria-label="Username" aria-describedby="basic-addon1">
                    <a class="text-light text-decoration-none pt-1" href="#">SUBSCRIBE</a>
                </div>
                
            </div>
</template>

<script>
export default {
name: 'FooterContact',
props: ['menuTitle','location','phone','mail']
}
</script>

<style>

</style>