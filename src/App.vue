// Author : The Mufid

<template>
  <div id="login">
    <main>
        <Login />
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
  background: url("assets/background.jpg") center center;
  background-size: cover;
  width: 100%;
  height: 100%;
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
}
</style>
