<template>
<div class="card">
    <img :src="data.image_url" :alt="data.name">
    <div class="detalis">
        <h2>{{ data.name }}</h2>
        <p>{{ data.age }}</p>
        <p>{{ data.major }}</p>
        <p>{{ data.address }}</p>
        <button v-on:click="getContact(data.id)" class="primaryBtn btn">Contact Me!</button>
    </div>
</div>
</template>

<script>
export default {
    name: 'Student',
    props: {
        data: Object,
        getContact: Function
    }
}
</script>
