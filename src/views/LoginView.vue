<template>
  <div class="login">
    <h3>登录页面</h3>
    <div class="form">
      <el-form :model="formdata">
        <el-form-item>
          <el-input placeholder="用户名" v-model="formdata.user"></el-input>
        </el-form-item>
        <el-form-item>
          <el-input placeholder="密码" v-model="formdata.pw"></el-input>
        </el-form-item>
        <el-form-item>
          <el-button>提交</el-button>
        </el-form-item>
      </el-form>
    </div>
  </div>
</template>

<script>
export default {
  name: "LoginView",
  data() {
    return {
      formdata: {
        user: "admin",
        pw: 123456,
      },
    };
  },
};
</script>

<style scoped>
.login {
  width: 100vw;
  height: 100vh;
  background: rgb(224, 222, 222);
}
.login h3 {
  text-align: center;
  margin: 50px 50px;
}
</style>