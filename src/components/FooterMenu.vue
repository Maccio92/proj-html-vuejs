<template>
    <li><a class="text-decoration-none features-caption" :href="link">{{name}}</a></li>
</template>

<script>
export default {
name: 'FooterMenu',
props: ['link', 'name']
}
</script>

<style>

</style>