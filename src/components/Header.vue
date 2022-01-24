<template>
<header>
    <div class="container-fluid h-100">
        <div class="row row-cols-12 h-100 justify-content-between align-items-center">
        <img class="col-1" src="../assets/img/logo-img-01.png" alt="logo everlead">
        <ul class="list-unstyled list-inline col-5 d-flex align-items-center m-0">
                <li class="list-inline-item">homes</li>
                <li class="list-inline-item">pages</li>
                <li class="list-inline-item">blog</li>
                <li class="list-inline-item">shop</li>
                <li class="list-inline-item">events</li>
                <li class="list-inline-item">elements</li>
                <i class="fas fa-search "></i>
                <i class="fas fa-list l"></i>
        </ul>
        </div>
    </div>
</header>
</template>

<script>
export default {
name: 'Header',
}
</script>

<style lang="scss">
img{
    width: 20%;
}
li{
    text-transform: uppercase;
}
</style>