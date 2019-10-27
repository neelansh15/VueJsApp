<template>
    <section class="hero is-primary is-bold is-fullheight">
        <div class="hero-body">
            <div class="container">
                <form v-on:submit="dothis">
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
                            <button class="button is-primary">Submit</button>
                        </div>
                    </div>
                </form>
            </div>
        </div>
    </section>
</template>

<script>
export default {
  name: 'Login',
  methods: {
    dothis (e) {
      e.preventDefault()
      alert(this.username + ' ' + this.password)
    }
  }
}
</script>

<style scoped>

</style>
