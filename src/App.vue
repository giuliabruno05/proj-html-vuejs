<script>
import PageHeader from './components/PageHeader.vue';
import PageMain from './components/PageMain.vue';
import PageFooter from './components/PageFooter.vue';
export default {
  components: {
    PageHeader,
    PageMain,
    PageFooter

  },
  data() {
    return {
      links: [
        {
          text: "HOME",
          url: "#"
        },
        {
          text: "PAGES",
          url: "#"
        },
        {
          text: "MENU",
          url: "#special"
        },
      ],
      menu: [
        {
          text: "EVENT",
          url: "#events"
        },
        {
          text: "BLOG",
          url: "#team"
        },
        {
          text: "LANDING",
          url: "#preOrder"
        }
      ]

    }
  },
}
</script>

<template>
  <PageHeader :details="links" :element="menu" />
  <PageMain />
  <PageFooter />
</template>

<style lang="scss">
@use './styles/general.scss' as *;
</style>
