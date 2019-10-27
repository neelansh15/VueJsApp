<template>
  <div>
    <Register v-on:register = addToList />
    <Registrations :user_list = this.users />
  </div>
</template>

<script>
import Register from './components/Register'
import Registrations from './components/Registrations'

export default {
  name: 'app',
  components: {
    Register, Registrations
  },
  data () {
    return {
      users: [
        // Test Data
        // {
        //   id: 1,
        //   username: 'neelansh',
        //   password: 'mathur'
        // },
        // {
        //   id: 2,
        //   username: 'Noice',
        //   password: 'yayy'
        // }
      ]
    }
  },
  methods: {
    addToList (user, pass) {
      this.users.push({
        id: Math.round(Math.random() * 1000),
        username: user,
        password: pass
      })
    }
  }
}
</script>

<style lang="scss">
@import './assets/bulma.min.css';
</style>
