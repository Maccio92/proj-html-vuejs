<template>
<header>
    <div class="container-fluid h-100">
        <div class="row row-cols-12 h-100 justify-content-between align-items-center">
        <img class="col-1" src="../assets/img/logo-img-01.png" alt="logo everlead">
        <ul class="list-unstyled list-inline col-5 d-flex align-items-center justify-content-end m-0">
                <li class="list-inline-item mx-4">homes</li>
                <li class="list-inline-item mx-4">pages</li>
                <li class="list-inline-item mx-4">blog</li>
                <li class="list-inline-item mx-4">shop</li>
                <li class="list-inline-item mx-4">events</li>
                <li class="list-inline-item mx-4">elements</li>
                <i class="fas fa-search list-inline-item mx-4"></i>
                <i class="fas fa-list list-inline-item mx-4"></i>
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
li{
    text-transform: uppercase;
    font-size: 0.7em;
    font-weight: 700;
}
</style>