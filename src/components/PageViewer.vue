<template>
  <div class="container">
    <h1>{{ page.pageTitle }}</h1>
    <p>{{ page.content }}</p>
    mastoLink
  </div>
</template>

<script>
export default {
  props: ['page']
}
</script>
