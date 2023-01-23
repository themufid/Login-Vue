// Author : The Mufid

<template>
  <div id="login">
    <main>
      <layout>
        <Login />
      </layout>
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
  background-size: repeat;
  width: 100%;
  height: 100%;
  position: absolute;
  top: 2;
  right: 2;
  bottom: 2;
  left: 2;
}
</style>
