<template>
  <div class="login-container">
    <div class="login-box">
      <div class="avatar-box">
        <img src="../assets/logo.png">
      </div>
      <!--登录表单-->
      <el-form ref="loginRef"  class="login-form">
        <!---用户名-->
        <el-form-item prop="=username">
          <el-input placeholder="用户名" prefix-icon="iconfont icon-user"></el-input>
        </el-form-item>

        <!--密码-->
        <el-form-item prop="password">
          <el-input placeholder="密码"  prefix-icon="iconfont icon-3702mima" type="password"
                    show-password></el-input>
        </el-form-item>

        <el-form-item class="btns">
          <el-button plain type="primary">登录</el-button>
          <el-button plain type="info">注册</el-button>
        </el-form-item>
      </el-form>
    </div>
  </div>
</template>

<script>
export default {
  name: 'LoginView'
}
</script>

<style scoped>
.login-container {
  background-color: #2b4b6b;
  height: 100%;
}

.login-box {
  width: 450px;
  height: 300px;
  background-color: #fff;
  border-radius: 3px;
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
}

.avatar-box {
  height: 130px;
  width: 130px;
  border: 1px solid #eee;
  border-radius: 50%;
  padding: 10px;
  box-shadow: 0 0 10px #ddd;
  position: absolute;
  left: 50%;
  transform: translate(-50%, -40%);
  background-color: #fff;
}

.avatar-box img {
  width: 100%;
  height: 100%;
  border-radius: 50%;
  background-color: #eee;
}

.btns {
  display: flex;
  justify-content: flex-end;
}

.login-form {
  position: absolute;
  bottom: 0;
  width: 100%;
  padding: 0 20px;
  box-sizing: border-box;
}
</style>
