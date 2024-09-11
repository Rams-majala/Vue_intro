<template>
    <nav v-bind:class="{active: isActive, }">
        <ul>
            <li>Home</li>
            <li>About</li>
            <li>Service</li>
            <li>Contact</li>
        </ul>
    </nav>
</template>

<script>
    export default {
        name: 'MainLaylout',
        isActive: false
    }
</script>

<style scoped>
nav{
    padding: 20px;
    background-color: darkgray;
    display: flex;
    justify-content: end;

}
ul li{
    list-style: none;
    display: inline;
    padding: 10px;
}

</style>