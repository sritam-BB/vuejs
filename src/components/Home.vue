<template>
<h1 class="tCenter">Student Details</h1>
<div class="Grid4">
    <div v-for="item in students" :key="item.id">
        <Student :data="item" :getContact="getContact" />
    </div>
</div>
</template>

<script>
import Student from './Student';

export default {
    name: "Home",
    components: {
        Student
    },
    methods: {
        getContact(id) {
            alert("Hey, This is your student id " + id);
        }
    },
    data() {
        return {
            students: [{
                    id: "01",
                    name: "John Doe",
                    age: "25",
                    major: "Computer Science",
                    image_url: "https://dummyimage.com/300x300/000/fff&text=John+Doe",
                    address: "123 Main Street, Anytown, USA"
                },
                {
                    id: "02",
                    name: "Alice Smith",
                    age: "28",
                    major: "Electrical Engineering",
                    image_url: "https://dummyimage.com/300x300/000/fff&text=Alice+Smith",
                    address: "456 Elm Avenue, Othertown, USA"
                },

                {
                    id: "03",
                    name: "Michael Johnson",
                    age: "22",
                    major: "Psychology",
                    image_url: "https://dummyimage.com/300x300/000/fff&text=Michael+Johnson",
                    address: "789 Oak Lane, Anycity, USA"
                },

                {
                    id: "05",
                    name: "David Lee",
                    age: "26",
                    major: "Biology",
                    image_url: "https://dummyimage.com/300x300/000/fff&text=David+Lee",
                    address: "246 Maple Avenue, Newville, USA"
                },

            ]
        }
    }
}
</script>

<style>
@import '../css/utils.css';
</style>
