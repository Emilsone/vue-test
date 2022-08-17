
<template functional>
  <section id="shopping-app">
    <div class="shopping-app">
      <div class="container-text">
        <div class="text">
          <h1>Shopping List</h1>
        </div>
      </div>
      <div class="list">
        <p v-for="item in props.items" :key="item">{{ item}}</p>
      </div>

      <!-- <p class="footer">Made With ❤ ❤ ❤ By Emilson</p> -->
    </div>
  </section>
</template>
<script>
export default {
  functional: true,
  name: "ListItem",
  props: {
    items: Array,
  },
};
</script>
<style scoped>
.form-box > .input-box > .label > .icon-mouse {
  padding: 0px 20px;
}
.form-box {
  display: flex;
  justify-content: space-between;
  align-items: center;
  color: #aaaaaa;
  margin: 10px 0px;
}

#shopping-app {
  display: flex;
  justify-content: center;
}
.fa-plus {
  background-color: #fca954;
  color: #ffffff;
  width: 40px;
  height: 40px;
  display: flex;
  justify-content: center;
  align-items: center;
  border-radius: 30px;
}
.icon-font {
  font-size: 40px;
  color: #fca954;
}
.icon-font:hover {
  transition: all 0.3s ease-in-out;
}
.btn {
  color: green;
}
.list {
  width: 300px;
  /* border: 1px solid black; */
  display: flex;
  flex-direction: column;
  padding: 20px;
  background: #444444;
}
.container {
  width: 300px;
  /* border: 1px solid black; */
  display: flex;
  /* flex-direction: column; */
  justify-content: space-between;
  align-items: center;
  padding: 20px;
  margin: 10px 0px;
  background: #444444;
  color: #ffffff;
}
.container input {
  width: 80%;
  padding: 8px 0px;
  outline: none;
  background: transparent;
  border: none;
  color: #ffffff;
  font-size: 17px;
}
::placeholder {
  color: #ffffff;
}
.container-text {
  width: 300px;
  /* border: 1px solid black; */
  padding: 20px;
  margin: 20px 0px;
  background: #444444;
  color: #ffffff;
}
.text {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.footer {
  color: #aaaaaa;
  padding: 10px 0px;
  text-align: center;
}
.icon-mouse {
  cursor: pointer;
}
@media (max-width: 332px) {
  .list,
  .container-text,
  .container {
    width: 270px;
    max-width: 250px;
  }
}
</style>








