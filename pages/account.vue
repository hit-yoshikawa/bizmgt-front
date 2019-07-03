<template>
  <v-layout
    column
    justify-center
    align-center
  >
    <v-flex
      xs12
      sm8
      md6
    >
      <div>
        <v-btn flat @click="user">
          ユーザー
        </v-btn>
      </div>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  methods: {
    user: function () {
      this.$router.push('/user')
    }
  }
}
</script>
