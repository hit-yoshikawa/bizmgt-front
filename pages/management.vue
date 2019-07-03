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
        <v-btn flat @click="project">
          プロジェクト
        </v-btn>
        <v-btn flat @click="memberAssign">
          アサイン
        </v-btn>
        <v-btn flat @click="customer">
          顧客
        </v-btn>
        <v-btn flat @click="company">
          企業
        </v-btn>
        <v-btn flat @click="member">
          メンバ
        </v-btn>
      </div>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  methods: {
    project: function () {
      this.$router.push('/project')
    },
    memberAssign: function () {
      this.$router.push('/member-assign')
    },
    customer: function () {
      this.$router.push('/customer')
    },
    company: function () {
      this.$router.push('/company')
    },
    member: function () {
      this.$router.push('/member')
    }
  }
}
</script>
