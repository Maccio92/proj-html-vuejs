<template>
    <li class="list-inline-item mx-4 nav-item">
        <a :href="value">{{name}}</a>
    </li>
</template>

<script>
export default {
    name: 'Navigation',
    props: ["name", "value"]

}
</script>

<style lang="scss" scoped>
.nav-item {
    text-transform: uppercase;
    font-size: 0.7em;
    font-weight: 700;
    a{
    color: black;
    text-decoration: none;
    }
}
</style>