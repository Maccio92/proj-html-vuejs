<template>
<header>
    <div class="container-fluid h-100">
        <div class="row row-cols-12 h-100 justify-content-between align-items-center">
        <img class="col-1" src="../assets/img/logo-img-01.png" alt="logo everlead">
        <ul class="list-unstyled list-inline col-5 d-flex align-items-center justify-content-end m-0">
            <Navigation
            v-for="(item, index) in navItem"
            :key="index"
            :name="item.name"
            :value="item.href"
            />
                <i class="fas fa-search list-inline-item mx-4"></i>
                <i class="fas fa-list list-inline-item mx-4"></i>
        </ul>
        </div>
    </div>
</header>
</template>

<script>
import Navigation from './Navigation.vue';

export default {
components: { 
    Navigation 
    },
name: 'Header',
data(){
        return{
            navItem: [{
                    href: "#",
                    name: "homes",
                },
                {
                    href: "#",
                    name: "pages",
                },
                {
                    href: "#",
                    name: "blog",
                },
                {
                    href: "#",
                    name: "shop",
                },
                {
                    href: "#",
                    name: "events",
                },
                {
                    href: "#",
                    name: "elements",
                },
            ]
        }
    }
}
</script>

<style lang="scss">

</style>