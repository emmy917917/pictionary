<template lang='pug'>
b-navbar(toggleable, type='inverse', variant='primary', fixed)
  b-nav-toggle(target='nav_collapse_example')
  .container
    b-link.navbar-brand(to='/')
      span Pictionary
    b-collapse#nav_collapse_example(is-nav)
      b-nav.ml-auto(is-nav-bar)
        b-nav-item(to='/lobby') Play
        b-nav-item(to='/game') Game
</template>

<script>
export default {
  name: 'navbar'
}
</script>

<style lang='scss'>
.navbar-toggler {
  z-index: 100;
}
</style>