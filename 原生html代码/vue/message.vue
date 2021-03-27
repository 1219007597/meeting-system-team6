<template>
  <el-card class="box-card">
    <h2>信息发布</h2>
    <el-form ref="form" :model="form" label-width="80px">
      <el-form-item label="标题" class="input1">
        <el-input v-model="form.title"></el-input>
      </el-form-item>
      <el-form-item label="内容">
        <el-input type="textarea" v-model="form.content" class="input2"></el-input>
      </el-form-item>
      <el-form-item>
        <el-button type="primary" @click="onSubmit">立即发布</el-button>
        <el-button @click="rest">重置</el-button>
      </el-form-item>
    </el-form>
  </el-card>
</template>

<style scoped>
.box-card {
  width: 700px;
}

</style>

<script>
export default {
  data() {
    return {
      form: {
        title: "",
        content: ""
      }
    };
  },
  methods: {
    onSubmit() {
      console.log("submit!");
    },
    rest() {
      (this.form.title = ""), (this.form.content = "");
    }
  }
};
</script>
