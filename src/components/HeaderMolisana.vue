<template>
  <header>
    <div class="container">
      <img src="@/assets/img/la-molisana-logo.png" alt="">
      <ul>
        <li @click="setActiveIndex(index)" v-for="(link, index) in links" :key="link.text" :class="{active: index == activeIndex}">
          <a :href="link.href">{{ link.text }}</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<script>
export default {
  name: 'HeaderMolisana',
  data () {
    return {
      activeIndex: 1,
      links: [
        {
          href: '#',
          text: 'Home'
        },
        {
          href: '#',
          text: 'Prodotti'
        },
        {
          href: '#',
          text: 'Chi siamo'
        },
        {
          href: '#',
          text: 'Contatti'
        }
      ]
    }
  },
  methods: {
    setActiveIndex (index) {
      this.activeIndex = index
    }
  }
}
</script>

<style scoped lang="scss">
@import "@/assets/styles/partials/variables";
.container {
  text-align: center;
}

li {
  display: inline-block;
  padding: 1rem;
  &.active {
    background-color: $active_color;
  }
  a {
    display: inline-block;
    text-decoration: none;
  }
}
</style>
