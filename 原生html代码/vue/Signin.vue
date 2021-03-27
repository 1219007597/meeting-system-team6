<template>
  <div class="login">
    <div class="top">
      <h1>注册</h1>
    </div>
    <div class="ref">
      <p>
        用户名：
        <input type="text" id="input" />
      </p>
    </div>
    <div class="refp">
      <p>
        密码：
        <input type="password" id="input" />
      </p>
    </div>
    <div class="re">
      <el-select v-model="value1" multiple placeholder="请选择">
        <el-option
          v-for="item in options"
          :key="item.value"
          :label="item.label"
          :value="item.value"
        ></el-option>
      </el-select>
    </div>
    <div class="button">
      <button id="lg">确认注册</button>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      input: "",
      options: [
        {
          value: "选项1",
          label: "黄金糕"
        },
        {
          value: "选项2",
          label: "双皮奶"
        },
        {
          value: "选项3",
          label: "蚵仔煎"
        },
        {
          value: "选项4",
          label: "龙须面"
        },
        {
          value: "选项5",
          label: "北京烤鸭"
        }
      ],
      value1: []
    };
  }
};
</script>
<style scoped>

.re{
  padding-top: 20px;
}



body {
  text-align: left;
}
.login {
  width: 350px;
  height: 370px;
  background-color:#9ddfd3;
  margin: 150px auto;
  font-weight: 900;
  border: 1px #eee solid;
}
.top {
  width: 100%;
  height: 50px;
  background-color:#9ddfd3;
  float: left;
  color: black;
  text-align: center;
  line-height: 50px;
}
.ref {
  width: 280px;
  height: 40px;
  margin-top: 20px;
  margin-left: 25px;
  float: left;
  text-align: center;
  line-height: 40px;
}
.refp {
  width: 280px;
  height: 40px;
  margin-top: 20px;
  margin-left: 25px;
  letter-spacing: 5px;
  float: left;
  text-align: center;
  line-height: 40px;
}
.re {
  width: 280px;
  height: 40px;
  margin-top: 20px;
  margin-left: 45px;
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

.button {
  margin-top: 300px;
  margin-left: 10px;
  padding-left: 120px;
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
}

.shortselect {
  background: #fafdfe;
  height: 60px;
  width: 180px;
  line-height: 28px;
  border: 1px solid #9bc0dd;
  -moz-border-radius: 2px;
  -webkit-border-radius: 2px;
  border-radius: 2px;
}
</style>