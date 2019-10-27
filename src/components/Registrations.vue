<template>
    <section class="hero is-fullheight is-dark is-bold">
       <div class="hero-body">
           <div class="container has-text-centered">
                <span>Registered Users:</span>
                <ul>
                    <div v-for="user in user_list" :key="user.id">
                        <li>{{ user.username }}</li>
                    </div>
                </ul>
           </div>
       </div>
    </section>
</template>

<script>
export default {
  name: 'Registrations',
  props: ['user_list']
}
</script>

<style scoped>

</style>
