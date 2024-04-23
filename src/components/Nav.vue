<template>
<div class="navBar">
    <div class="logo">
        <img alt="Vue logo" src="../assets/logo.png">
    </div>
    <ul>
        <li>Home</li>
        <li>About</li>
        <li>Contact</li>
    </ul>
</div>
</template>

<script>
export default {
    name: 'Nav'
}
</script>

<style scoped>
@import '../assets/css/utils.css';
.navBar {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 1.5rem 4rem;
}

.logo {
    width: 50px;
    cursor: pointer;
}

.logo img {
    width: 100%;
}
.navBar ul{
    display: flex;
    flex-direction: row;
}
.navBar ul li{
    padding: 0 1rem;
    list-style: none;
    cursor: pointer;
}
</style>
