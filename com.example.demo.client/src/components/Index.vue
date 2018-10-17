<template>
  <div>
    <el-button type="primary" @click="init">刷新</el-button>
    {{tableData}}
  </div>
</template>

<script>
export default {
  name: "Index",
  data() {
    return {
      tableData: ""
    };
  },
  mounted() {
    this.init();
  },
  methods: {
    init() {
      this.$axios.get("/ok").then(res => {
        this.tableData = res.data;
        console.log(this.tableData)
      });
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
