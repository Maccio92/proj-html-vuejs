<template>
<li class="d-flex mb-5 ">
    <div class="data-container d-flex flex-column justify-content-center align-items-center">
        <p class="data">{{day}}</p>
        <p class="data-light">{{date}}</p>
    </div>
    <div class="ps-3">
        <h4 class="features-title">{{eventTitle}}</h4>
        <div class="d-flex align-items-center">
            <i class="far fa-clock text-orange"></i>
            <p class="m-0 ps-2">{{time}}</p>
        </div>
        <div class="d-flex align-items-center mb-2 ">
            <i class="fas fa-map-marker-alt text-orange"></i>
            <p class="m-0 ps-2">{{address}}</p>
        </div>
        <a class="text-decoration-none text-dark fw-bolder" href="#">Read More</a>
    </div>
</li>
</template>

<script>
export default {
name:'Event',
props:['day','date','eventTitle','time','address'],
}
</script>

<style>

</style>
