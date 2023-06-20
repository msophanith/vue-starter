<template>
  <form>
    <label>Email:</label>
    <input type="email" required v-model="email" />
    <label>Password:</label>
    <input type="password" required v-model="password" />
  </form>
  <div style="display: flex;flex-direction: column;">
    <span>Output</span>
    <span>Email: {{ email }}</span>
    <span>Password: {{ password }}</span>
  </div>
</template>

<script>
export default {
  data() {
    return {
      email: "",
      password: "",
    };
  },
};
</script>

<style scoped>
form {
  display: flex;
  flex-direction: column;
  background-color: aliceblue;
  padding: 20px;
  width: 50%;
  margin: 0 auto;
}
input {
  padding: 10px;
  border-radius: 5px;
  margin-bottom: 10px;
}
label {
  display: flex;
  font-weight: 600;
  color: darksalmon;
}
</style>
