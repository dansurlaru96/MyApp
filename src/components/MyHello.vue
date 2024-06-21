<script>
export default {
  name: "MyHello",
  setup() {
    return {
      msg: "First APP",
    };
  },
};
</script>

<template>
  <div class="myTitle">
    <h1>My First APP</h1>
    <p>Acesta este primul component creat</p>
  </div>
</template>

<style>
.myTitle {
  background-color: #f4f4f4;
  padding: 20px;
  border-bottom: 3px solid #ccc;
  text-align: center;
}
</style>
