<template>
  <AppHeader v-bind:apptitle="message" v-on:change="chanageMessage"></AppHeader>
</template>

<script>

import AppHeader from './components/AppHeader.vue'
export default {
  components: {
  AppHeader: AppHeader
  },

  data() {
    return {
    message: '앱 헤더 컴포넌트'
    }
  },
  methods: {
    chanageMessage() {
      this.message = '변경됨'
    }
  }
}
</script>

<style scoped>

</style>