<template>
  <nav>
    <div>
      <a href="#">pepe's website</a>
      <ul>
        <li v-for="(page, index) in pages" :key="index">
          <a
            :class="{ active: activepage == index }"
            aria-current="page"
            :title="`go to the ${page.link.text} page`"
            @click.prevent="navLinkClick(index)"
            >{{ page.link.text }}</a
          >
        </li>
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  props: ['pages', 'activePage', 'navLinkClick']
}
</script>
