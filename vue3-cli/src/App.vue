<template>
  <AppHeader></AppHeader>
  <div>
    {{ message }}
  </div>
  <button @click="showAlert">인사</button>
</template>

<script>

import AppHeader from './components/AppHeader.vue'
export default {
  components: {
  AppHeader: AppHeader
  },

  data() {
    return {
    message: 'hi'
    }
  },
  methods: {
    showAlert() {
      alert('hello')
    }
  }
}
</script>

<style scoped>

</style>