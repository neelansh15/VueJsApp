<template>
  <div>
    <Login />
    <Registrations />
  </div>
</template>

<script>
import Login from './components/Login'
import Registrations from './components/Registrations'

export default {
  name: 'app',
  components: {
    Login, Registrations
  },
  data () {
    return {

    }
  }
}
</script>

<style lang="scss">
@import './assets/bulma.min.css';
</style>
