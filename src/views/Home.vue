<template>
  <div class="home">
    <LoginPage/>
  </div>
</template>

<script>
// @ is an alias to /src
import { mapState } from 'vuex'
import LoginPage from '@/components/LoginPage.vue'

export default {
  name: 'Home',
  components: {
    LoginPage
  },
  computed: {
    ...mapState("auth", ['nome'])
  }
}
</script>
