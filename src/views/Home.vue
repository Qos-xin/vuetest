<template>
<div>
    <Nav/>
    <router-view/>
</div>
</template>

<script>
// @ is an alias to /src
import Nav from '@/components/Nav.vue'
export default {
  name: 'home',
  components: {
    Nav
  }
}
</script>
