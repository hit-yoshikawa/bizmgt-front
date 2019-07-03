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
        <v-btn flat @click="inquiry">
          引合
        </v-btn>
        <v-btn flat @click="estimate">
          見積
        </v-btn>
        <v-btn flat @click="order">
          受注
        </v-btn>
        <v-btn flat @click="invoice">
          請求
        </v-btn>
      </div>
    </v-flex>
  </v-layout>
</template>

<script>
export default {
  methods: {
    inquiry: function () {
      this.$router.push('/inquiry')
    },
    estimate: function () {
      this.$router.push('/estimate')
    },
    order: function () {
      this.$router.push('/order')
    },
    invoice: function () {
      this.$router.push('/invoice')
    }
  }
}
</script>
