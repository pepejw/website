<template>
  <div class="container">
    <h1>{{ page.pageTitle }}</h1>
    <p>{{ page.content }}</p>
    <a rel="me" href="https://tech.lgbt/@aeron69420">Mastodon</a>
  </div>
</template>

<script>
export default {
  props: ['page']
}
</script>
