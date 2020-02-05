<template>
<div id="homepage">
          <adminHome v-if="this.role === 'Admin'"/>
          <userHome v-if="this.role === 'User'"/>
</div>
</template>

<script>
import adminHome from '../components/admin/home.vue'
import userHome from '../components/user/home.vue'

export default {
  name: 'homepage',
  data () {
    return {
      role: []
    }
  },
  components: {
    adminHome,
    userHome
  },
  mounted () {
    this.role = localStorage.getItem('pageDetails')
    if (localStorage.getItem('userdetails')) {
    } else {
      this.$router.replace({ name: 'login' })
    }
  } }
</script>
