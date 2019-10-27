<template>
    <section class="hero is-primary is-bold is-fullheight">
        <div class="hero-body">
            <div class="container">

                <div>
                    <h1>Register</h1>
                </div>

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
                            <button class="button is-primary">Register</button>
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
    }
  }
}
</script>

<style scoped>
label{
    color: white;
}
</style>
