<template>
    <section class="hero is-warning is-large">
        <div class="hero-body">
            <div class="container">

                <h1 class="title">Register</h1>

                <form v-on:submit="register">
                    <div class="field">
                        <label class="label">Username</label>
                        <div class="control">
                            <input type="text" name="username" placeholder="Username" v-model="username">
                        </div>
                    </div>

                    <div class="field">
                        <label class="label">Password</label>
                        <div class="control">
                            <input type="password" name="password" placeholder="Password" v-model="password">
                        </div>
                    </div>

                    <div class="field">
                        <div class="control">
                            <button class="button is-dark">Register</button>
                        </div>
                    </div>
                </form>
            </div>
        </div>
    </section>
</template>

<script>
export default {
  name: 'Register',
  methods: {
    register (e) {
      e.preventDefault()
      this.$emit('register', this.username, this.password)
      this.username = ''
      this.password = ''
    }
  }
}
</script>

<style scoped>
/* label{
    color: white;
} */
</style>
