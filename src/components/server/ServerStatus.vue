<template>
  <div>
    <p>Status Server : {{ status }}</p>
    <button @click="changeStatus">Change Status</button>
    <hr>
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      status: 'Critical'
    }
  },
  methods: {
    changeStatus() {
      this.status = 'Normal'
    }
  }
}
</script>

<style scoped>
p {
  color: tomato;
}
</style>
