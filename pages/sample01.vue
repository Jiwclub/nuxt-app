<template>
  <div>
    <h1>{{ age }}Hello {{ name }}</h1>
    <input type="text" :value="name">
  </div>
</template>
<script>
export default {
  // data เป็น function
  data () {
    setInterval(() => {
      this.name += '*'
    }, 1000)
    return {
      name: 'Test',
      age: '25'
    }
  }
}
</script>
