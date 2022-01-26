<template>
<div class="card col-3 border-0">
    <div class="crop w-100">
        <img class="w-100 " :src="image1" alt="">
    </div>
    <div class="crop-down w-100 position-relative ">
        <img class="w-100 position-absolute bottom-0 start-0" :src="image2" alt="">
    </div>
    <div class="bg-orange position-absolute d-flex align-items-center justify-content-center p-2 orange-label ">
            <i class="text-light fas fa-tag"></i>
            <p class="text-light m-0 ps-1">{{argument1}}, {{argument2}}</p>
    </div>
    <div class="d-flex align-items-center justify-content-start py-3 ">
            <i class="far fa-clock text-orange features-caption"></i>
            <p class="m-0 px-2 features-caption">{{publication}}</p>
            <i class="text-orange far fa-user features-caption"></i>
            <p class="m-0 ps-2 features-caption">{{author}}</p>
    </div>
    <h3 class="event-title">{{newsTitle}}</h3>
    <p class="features-caption">{{newsCaption}}</p>
    <a class="text-decoration-none text-dark fw-bolder" href="#">Read More</a>
</div>
</template>

<script>
export default {
name: 'News',
props: ['image1','image2','argument1','argument2','publication','author','newsTitle','newsCaption']
}
</script>

<style>

</style>