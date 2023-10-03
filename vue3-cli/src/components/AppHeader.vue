<template>
  <h1>{{apptitle}}</h1>
  <button @click="changeTitle">변경</button>
</template>

<script>
export default {
  props: ['apptitle'],
  methods: {
    changeTitle() {
      this.$emit('change');
    }
  }

}
</script>

<style scoped>

</style>