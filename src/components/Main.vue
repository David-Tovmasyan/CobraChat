<script setup>
function myAlert() {
    alert("message");
}

</script>

<template>
    <div class="container">
        <header @click="myAlert">Header</header>
        <main>Main</main>
    </div>
</template>

<style scoped>
header {
    background-color: yellow;

}

main {
    background-color: black;
}
</style>
