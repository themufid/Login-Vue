// Author : The Mufid
// Description : Login Form

<template>
  <div class="main" :style="mainStyle">
    <h2>Welcome to Login Form!</h2>
    <input
      type="text"
      name="username"
      id="username"
      placeholder="Username"
      :style="input" />
    <br />
    <input
      type="password"
      name="password"
      id="password"
      placeholder="Password"
      :style="input" />
    <br />
    <input
      type="button"
      value="LOGIN"
      class="button"
      id="done"
      :style="inputStyle" />
    <br />
    <img src="../assets/google.svg" href="#" alt="Google" />
    <img src="../assets/twitter.svg" href="#" alt="Twitter" />
    <img src="../assets/instagram.svg" href="#" alt="Instagram" />
    <img src="../assets/LinkedIn.svg" href="#" alt="LinkedIn" />
    <img src="../assets/github.svg" href="#" alt="Github" />
  </div>
</template>

<script>
export default {
  name: "App",
  props: {
    mainStyle: String,
    inputStyle: String,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Poppins&display=swap");

.main {
  background: rgba(255, 255, 255, 0.4);
  position: absolute;
  top: 20%;
  left: 30%;
  width: 40%;
  text-align: center;
  padding: 5px;
  border-radius: 3rem;
  box-shadow: 0px 0px 8px -5px #000000;
  padding-top: 3%;
  padding-bottom: 5%;
  font-family: "Poppins", sans-serif;
}
h1 {
  cursor: default;
  user-select: none;
}
input {
  border-radius: 3rem;
  border: none;
  padding: 10px;
  text-align: center;
  outline: none;
  margin: 10px;
  width: 30%;
  box-sizing: border-box;
  font-family: "Poppins", sans-serif;
  font-weight: 400;
}
input:hover {
  box-shadow: 0px 0px 8px -5px #100001;
}
input:active {
  box-shadow: 0px 0px 8px -5px #100001;
}
#done {
  background: rgb(144, 196, 238);
}
.button {
  cursor: pointer;
  user-select: none;
}
img {
  height: 2.2rem;
  margin: 10px;
  user-select: none;
}
img:hover {
  box-shadow: 0px 0px 8px -5px #000001;
  cursor: pointer;
  border-radius: 200rem;
}
</style>
