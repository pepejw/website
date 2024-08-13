<template>
  <navbar-main
    :pages="pages"
    :active-page="activePage"
    :nav-link-click="(index) => (activePage = index)"
  ></navbar-main>

  <page-viewer :page="pages[activePage]"></page-viewer>
</template>

<script>
import NavbarMain from './components/NavbarMain.vue'
import PageViewer from './components/PageViewer.vue'

export default {
  components: {
    NavbarMain,
    PageViewer
  },
  data() {
    return {
      activePage: 0,
      pages: [
        {
          link: { text: 'home' },
          pageTitle: 'homepage',
          content: "welcome to pepe's website!"
        },
        {
          link: { text: 'contact' },
          pageTitle: 'contact me',
          content: 'reach out to me at pepejw@proton.me!'
        }
      ]
    }
  }
}
</script>
