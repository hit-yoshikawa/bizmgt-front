<template>
  <v-app dark>
    <v-toolbar>
      <v-toolbar-title @click="home">BIZMGT</v-toolbar-title>
      <v-spacer />
      <v-toolbar-items>
        <v-btn flat @click="counting">
          計数管理
        </v-btn>
        <v-btn flat @click="management">
          プロジェクト管理
        </v-btn>
        <v-btn flat @click="account">
          アカウント管理
        </v-btn>
        <v-btn flat @click="logout">
          logout
        </v-btn>
      </v-toolbar-items>
    </v-toolbar>
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
    home: function () {
      this.$router.push('/home')
    },
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
      this.$router.push('/')
    }
  }
}
</script>
