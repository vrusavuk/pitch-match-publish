<template>
    <section class="bg">
    <container class="container">
    <h1>404</h1>
    <h2>Oops...&#9917</h2>
    <p>Try going to the <router-link to="/ru">home</router-link> page.</p> 
    <v-btn-toggle />
    </container>
    </section>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.bg {
    height: 800px;
    width: 1200;
    background-image: url("./../assets/soccer-field-2.jpeg");
    -webkit-background-size: cover;
    -moz-background-size: cover;
    -o-background-size: cover;
    background-size: cover;
}

.container {
    justify-content: center;
    text-align: center;
}
.container h1 {
    font-size: 100px;
    font-weight: 500;
}
.container h2 {
    font-size: 30px;
    font-weight: 400;
    color: rgb(122, 122, 122);
}

.container p {
    font-size: 23px;
    font-weight: 300;
    
}
</style>