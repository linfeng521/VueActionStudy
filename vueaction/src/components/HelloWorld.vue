<template>
  <div class="hello">
    <h1>{{ msg }}</h1>
    <hr />
    <h2>{{ name }}</h2>
    <el-button @click="showMsg">点击</el-button>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  },
  data() {
    return {
      name: "linfeng  github action 学习"
    }
  },
  methods: {
    showMsg() {
      this.name = "linfeng521";
      this.$message({
        message: `恭喜${this.name}，这是一条成功消息`,
        type: 'success'
      });
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
}
</style>
