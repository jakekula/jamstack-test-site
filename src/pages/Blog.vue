<template>
    <Layout>
        <div>
            <div v-for="edge in $page.posts.edges" :key="edge.node.id">
                <h2>{{ edge.node.title }}</h2>
                <p>Some text</p>
            </div>
        </div>
    </Layout>
</template>

<page-query>
query Posts {
    posts: allContentfulBlogPost {
        edges {
            node {
                id,
                title,
                description,
                date (format: "MMMM DD, YYYY"),
                path
            }
        }
    }
}
</page-query>

<script>
export default {
    metaInfo: {
        title: 'Blog'
    }
}
</script>