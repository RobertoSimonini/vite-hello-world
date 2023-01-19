<script>
export default {
    name: 'App Hero',
    data() {
        return {
            images: ['logo-marvel.webp', 'altro-logo-marvel.jpg' ]
        }
    },

    methods: {
        buildImagePath (image) {
            const url = new URL(`../assets/${image}`, import.meta.url);
            return (url.href);
        }
    }
}
</script>

<template>
    <ul>
        <li v-for="image in images">
            <img :src="buildImagePath(image)" alt="">
        </li>
    </ul>
</template>


<style scoped>
    ul {
        list-style-type: none;
        text-align: center;
    }
</style>