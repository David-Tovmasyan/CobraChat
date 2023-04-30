<script setup>

import Form from './Form.vue';
function myAlert() {
    alert("message");
}

</script>

<template>
    <div class="page_container">
        <header @click="myAlert">
          <img src="/logo.png" alt="Logo" class="logo">
          
        </header>
        <main>
          <div class="list">
            <div className="searchBar">
                <input type="search" placeholder="Search" class="Search">
            </div>
          </div>
        </main>
          
        <footer>Footer</footer>
    </div> 
    <Form></Form> 
</template>

<style scoped>

.page_container{
  display: grid;
  grid-template-rows: 100px calc(100vh - 100px - 40px) 40px;
}
header{
  height: 100px;
  display: flex;
  justify-content: center;
  background-image: linear-gradient(to right,rgb(4, 105, 42), rgb(58, 245, 51));
}
.logo{
  width: 250px;
  height:50px;
  margin-top: 20px;
  
}

.Search {
    background-color: rgb(196, 196, 196);
    border-radius: 10px;
    border: 1px solid black;
    max-width: 18em;
}


</style>
