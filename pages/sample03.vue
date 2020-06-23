<template>
  <div>
    <h1>{{ age }}Hello {{ name }}</h1>
    <h2>{{ upperNmae }}</h2>
    <input type="text" :value="name">
    <br>
    <input v-model="name" type="text">
    <br>
    <input v-model="name" type="text">
  </div>
</template>
<script>
export default {
  // data เป็น function
  data () {
    // setInterval(() => {
    //   this.name += '*'
    // }, 1000)
    return {
      name: 'Test',
      age: 25
    }
  },
  // computed ไม่ใช่ฟังค์ชั่น
  computed: {
    upperNmae () {
      return this.name.toUpperCase()
    }
  }
}
</script>
