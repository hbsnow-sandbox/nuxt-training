<template>
  <section class="container">
    <div>
      hoge
    </div>
  </section>
</template>

<script>
export default {
  async mounted() {
    const json = await this.$axios.$get('https://qiita.com/api/v2/items?query=tag:nuxt.js')
    console.log(json)
  }
}
</script>
