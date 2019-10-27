<template>
    <div class="container">
        <div class="hero">
            <div class="hero-body">
                <form>
                    <div class="field">
                        <label class="label">Username</label>
                        <div class="control">
                            <input type="text" name="username" placeholder="Username">
                        </div>
                    </div>

                    <div class="field">
                        <label class="label">Password</label>
                        <div class="control">
                            <input type="text" name="password" placeholder="Password">
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
    </div>
</template>

<script>
export default {
  name: 'Login'
}
</script>

<style scoped>

</style>
