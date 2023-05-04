<script setup>
import Form from './Form.vue';
</script>

<template>
  <div class="page_container">
    <header>
      <img src="/logo.png" alt="Logo" class="logo">

    </header>
    <main>

      <div class="contacts">
        <div class="searchBar">
          <input type="search" placeholder="Search" class="Search">
        </div>
      </div>
      <div class="line"></div>
      <div class="chat">
        <div class="info">
          <div class="nickname"></div>
          <div class="settings"></div>
        </div>
      </div>
    </main>


  </div>
  <Form></Form>
</template>

<style scoped>
.page_container {
  display: grid;
  grid-template-rows: 100px calc(100vh - 100px);
}

header {
  height: 100px;
  display: flex;
  justify-content: center;
  background-image: linear-gradient(to right, rgb(46, 147, 85), rgb(58, 245, 51), rgb(46, 147, 85));
}

.logo {
  width: 250px;
  height: 50px;
  margin-top: 20px;

}

main {
  display: grid;
  grid-template-columns: 20% 80%;
  grid-template-rows: 100%;
}

.contacts {
  display: flex;
  justify-content: center;
}

.Search {
  background-color: rgb(2, 255, 124);
  border-radius: 10px;
  border: 1px solid blue;
  width: 150px;
  height: 25px;
}

.line {
  display: inline-block;
  background-color: rgb(86, 206, 86);
  width: 5px;
  height: 100%;
}
</style>
