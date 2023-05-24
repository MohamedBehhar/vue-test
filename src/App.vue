<script >
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import user from "./assets/user.json"

export default {
  data(){
    return {
      users: user
    }
  }
}
</script>

<template>
  <div>
    <div  v-for="(user, id) in users" :key="id">
      <h1>{{ user.name }}</h1>
      <p>Age: {{  user.age}}</p>
    </div>
  </div>

</template>

<style scoped>


</style>
