<template>
    <v-container>
        <h1>Blog Posts</h1>
        <ul v-for="post in blogPosts" :key="post.title">
            <li> 
                <h2><nuxt-link :to="'/blog/' + post.slug"> {{ post.title }}</nuxt-link></h2>
                <p>{{ post.description }}</p>
            </li>
        </ul>
    </v-container>
</template>

<script>
export default {
    data() {
        return {
            post: {},
        }
    },
    computed: {
    blogPosts() {
      return this.$store.state.blogPosts;
    },
  },

}
</script>
