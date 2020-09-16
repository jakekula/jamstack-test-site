<template>
    <Layout>
        <div>
            <h1>{{$page.post.title}}</h1>
            <p>Posted on: {{$page.post.date}}</p>
            <p>{{$page.post.body}}</p>
        </div>
    </Layout>
</template>

<page-query>
query Post ($path: String!) {
    post: contentfulBlogPost (path: $path) {
        id,
        title,
        body,
        date (format: "MMMM DD, YYYY"),
        path
    }
}
</page-query>

<script>
import MarkdownIt from "markdown-it";

export default {
    computed: {
        body() {
            const md = new MarkdownIt();
            return md.render(this.$page.post.body);
        }
    }
}
</script>