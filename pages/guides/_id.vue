<template>
    <div>
        <h1>{{ guide.title }}</h1>
        <p>{{ guide.content }}</p>
    </div>
</template>

<script>
export default {
    data() {
        return {
            id: this.$route.params.id, // id is _id whatever we called the _something.vue
            guides: [
                {
                    id: "1",
                    title: "Guide 1",
                    content: "OMG"
                },
                {
                    id: "2",
                    title: "Pos 2",
                    content: ""
                },
                {
                    id: "3",
                    title: "",
                    content: ""
                }
            ]
        };
    },
    computed: {
        guide() {
            return this.guides.find(guide => guide.id);
        }
    }
};
</script>
