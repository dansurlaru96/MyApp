<script>
export default {
  setup() {
    return {
      count: ref(0),
    };
  },
};
</script>

<template>
  <div class="myApp">
    <h1 class="titleApp">ValueApp</h1>
    <div class="myInfo">
      <p>Numarul este;</p>
      <h1 class="myCount">{{ count }}</h1>
    </div>
    <div class="myBtnFlex">
      <button class="myBtn" @click="count++">Adauga</button>
      <button class="myBtn" @click="count = 0">Reset</button>
      <button class="myBtn" @click="count--">Scade</button>
    </div>
  </div>
</template>

<style>
.myApp {
  padding-top: 3%;
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}
.myCount {
  font-size: 10rem;
  color: rgb(30, 180, 50);
}
.myBtnFlex {
  display: flex;
  justify-content: center;
  margin-top: 10px;
  text-align: center;
  gap: 10px;
}
.myBtn {
  padding: 10px 20px;
  font-size: 1.5rem;
  background-color: rgb(188, 151, 2);
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}
.myBtn:hover {
  background-color: rgb(221, 176, 0);
}
</style>
