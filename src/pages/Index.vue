<template>
  <Layout>
    <div class="pt-24">
      <div class="container pb-20 px-3 mx-auto flex flex-wrap flex-col md:flex-row items-center">
        <!-- left column -->
        <div class="flex flex-col w-full md:w-2/5 justify-center justify-between text-center md:text-left pb-10">
          <p class="uppercase tracking-loose w-full text-primary">some heading here</p>
          <h1 class="py-4 text-5xl font-bold leading-tight w-full text-primary">Some text here blah blah blah</h1>
          <p class="leading-normal text-2xl pb-8 w-full text-primary">something here bzzzzttttttt</p>
          <g-link to="/blog">
            <button>Blog</button>
          </g-link>
        </div>
        <div class="w-full md:w-3/5 py-6 text-center">
          <img class="w-full md:w-5/5 z-50" src="../../static/images/undraw_Artificial_intelligence_re_enpp.svg" alt="something" />
        </div> 
      </div>
    </div>
  </Layout>
</template>

<script>
export default {
  metaInfo: {
    title: 'Home'
  }
}
</script>
