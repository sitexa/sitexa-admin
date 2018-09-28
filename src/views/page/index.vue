<template>
  <div class="app-container">
    <el-main class="el-main">
      <p> I love vue</p>
      <li class="decrease"> id: {{ id }}</li>
      <li class="decrease">name: {{ name }}</li>
      <li class="decrease">description: {{ desc }}</li>
    </el-main>
  </div>
</template>

<script>
export default {
  data() {
    return {
      id: '',
      name: '',
      desc: ''
    }
  },
  created() {
    this.fetchData()
  },
  methods: {
    fetchData() {
      this.id = '1'
      this.name = 'i have no name'
      this.desc = 'description'
    }
  }
}
</script>

<style scoped>
  .line{
    text-align: center;
  }
</style>
