<script setup>
function myAlert() {
    alert("message");
}

</script>

<template>
    <div class="page_container">
        <header @click="myAlert">
          <img src="/logo.png" alt="Logo" class="logo">
          
        </header>
        <main>Main</main>
        <footer>Footer</footer>
    </div>
</template>

<style scoped>

.page_container{
  display: grid;
  grid-template-rows: 100px calc(100vh - 100px - 40px) 40px;
}
header{
  background-color: #0ea47a;
  display: flex;
  justify-content: center;
}
.logo{
  width: 200px;
  height:100px;
  
}

</style>
