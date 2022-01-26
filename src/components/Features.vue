<template>
<li class="d-flex flex-column list-inline-item align-items-center col-3 p-3 m-0">
    <img class="p-5" :src="img" alt="">
    <h3 class="features-title">{{title}}</h3>
    <p class="features-caption text-center">{{caption}}</p>
</li>
</template>

<script>
export default {
name: 'Features',
props: ['img', 'title', 'caption']
}
</script>

<style lang="scss">

</style>