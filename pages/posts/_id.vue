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
                    id: 0,
                    title: "Post 1",
                    content: "MILK MILK"
                },
                {
                    id: 1,
                    title: "Pos 2",
                    content: ""
                },
                {
                    id: 2,
                    title: "",
                    content: ""
                }
            ]
        };
    },
    computed: {
        post() {
            return this.posts.find(post => this.id);
        }
    }
};
</script>
