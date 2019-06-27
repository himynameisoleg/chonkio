<template>
    <div>
        <h1>{{ post.title }}</h1>
        <p>{{ post.content }}</p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            id: this.$route.params.id, // id is _id whatever we called the _something.vue
            posts: [
                {
                    id: 'milk',
                    title: 'MILK',
                    content: 'MILK MILK'
                },
                {
                    id: '',
                    title: '',
                    content: ''
                },
                {
                    id: '',
                    title: '',
                    content: ''
                },
            ]
        }
    },
    computed: {
        post() {
            return this.posts.find(post => post.id);
        }
    }
}
</script>

<style scope>

</style>
