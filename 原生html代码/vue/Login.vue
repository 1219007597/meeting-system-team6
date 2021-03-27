<template>
  <div class="login">
    <div class="text">
      <h1>登录 </h1>
      <p>类型：</p>
      <el-select v-model="value" placeholder="请选择">
        <el-option
          v-for="item in options"
          :key="item.value"
          :label="item.label"
          :value="item.value"
        ></el-option>
      </el-select>
      <p>用户名：</p>
      <el-input v-model="name" class="input1" placeholder="请输入内容"></el-input>
      <p>密码：</p>
      <el-input v-model="password" class="input2" placeholder="请输入内容"></el-input>
    </div>
    <div class="buttonFace">
      <el-button type="primary" plain>登录</el-button>
      <el-button type="primary" plain>注册</el-button>
    </div>

  </div>
</template>
<script>
export default {
  data() {
    return {
      name: "",
      password: "",
      options: [
        {
          value: "选项1",
          label: "会议主席"
        },
        {
          value: "选项2",
          label: "论坛主席"
        },
        {
          value: "选项3",
          label: "普通参会者"
        }
      ],
      value: ""
    };
  }
};
</script>
<style scoped>

body {
  background: '../assets/7.png';
}

.text{
  width:100%;
  height: 80%;

}

.buttonFace{
  width:100%;
  height: 20%;
  padding-left: 100px;
}

.text h1{
  padding-left: 130px;
}



.el-select{
  width:200px;
  height: 50px;
  position: absolute;
  top: 80px;
  left: 100px;
}

.input1{
  width: 150px;
  height: 50px;
  position:absolute;
  top: 150px;
  left: 100px;
}


.input2{
  width: 150px;
  height: 50px;
  position:absolute;
  top: 220px;
  left: 100px;
}



.login {
  width: 350px;
  height: 370px;
  background-color:#9ddfd3;
  position: absolute;
  top: 150px;
  left: 600px;
}

.text p{
  width: 90px;
  height: 50px;
  padding-left: 20px;
  font-size: 18px;
}

/* 
.ref p{
  background-color: aqua;
  width: 80px;
  text-align: left;
  font-size: 20px;
} */
/* .top {
  width: 100%;
  height: 50px;
  background-color: white;
  float: left;
  color: black;
  text-align: center;
  line-height: 50px;
}
.ref {
  width: 280px;
  height: 40px;
  margin-top: 30px;
  margin-left: 20px;
  float: left;
  text-align: center;
  line-height: 40px;
}
#lg {
  width: 100px;
  height: 40px;
  font-size: 12pt;
  border: 1px #eee solid;
}
#res {
  width: 100px;
  height: 40px;
  font-size: 12pt;
  margin-left: 30px;
  border: 1px #eee solid;
}
.button {
  margin-top: 280px;
  margin-left: 10px;
}
#input {
  border: 1px solid #ccc;
  padding: 7px 0px;
  border-radius: 3px;
  padding-left: 5px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out 0.15s,
    -webkit-box-shadow ease-in-out 0.15s;
  -o-transition: border-color ease-in-out 0.15s, box-shadow ease-in-out 0.15s;
  transition: border-color ease-in-out 0.15s, box-shadow ease-in-out 0.15s;
}
#input:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075),
    0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075),
    0 0 8px rgba(102, 175, 233, 0.6);
} */
</style>