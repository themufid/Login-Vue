// Author : The Mufid

<template>
  <div id="login">
    <main>
      <mq-layout mq="sm">
        <Login mainStyle="left:10%;width:80%;" inputStyle="width:50%;" />
      </mq-layout>
    </main>
  </div>
</template>

<script>
import Login from "./components/Login.vue";

export default {
  name: "App",
  components: {
    Login,
  },
  mounted: async () => {
    await new Promise((r) => setTimeout(r, 3000));
    document.getElementById("white").classList.add("hidden");
    await new Promise((r) => setTimeout(r, 600));
    document.getElementById("white").remove();
  },
};
</script>

<style>
#login {
  background: url("assets/background.jpg") center;
  background-size: cover;
  width: 100%;
  height: 100%;
  position: absolute;
  top: 1;
  right: 2;
  bottom: 1;
  left: 2;
}
</style>
