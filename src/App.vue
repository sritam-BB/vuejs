<template>
<Nav />
<Home />
</template>

<script>
import Nav from './components/Nav.vue';
import Home from './components/Home.vue';

export default {
    name: 'App',
    components: {
        Nav,
        Home
    }
}
</script>
