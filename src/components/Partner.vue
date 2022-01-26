<template>
<li class="list-inline-item col-2 p-5">
    <img class="partner-img" :src="image" alt="">
</li>
</template>

<script>
export default {
name:'Partner',
props: ['image']
}
</script>

<style>

</style>