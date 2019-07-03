<template>
  <v-app dark>
    <v-content>
      <v-container>
        <nuxt />
      </v-container>
    </v-content>
  </v-app>
</template>

<script>
export default {
  methods: {
    counting: function () {
      this.$router.push('/counting')
    },
    management: function () {
      this.$router.push('/management')
    },
    account: function () {
      this.$router.push('/account')
    },
    logout: function () {
      alert('logout')
    }
  }
}
</script>
