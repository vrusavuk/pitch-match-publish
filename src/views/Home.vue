<template>
  
    <section class="intro-bg">  
      <div class="intro">
        <intro />
        <img class="img-fluid" src="./../assets/mocukup.png" alt="Pitch Match Mockup">
      </div>
    </section>
   
</template>

<script>
import Intro from './../components/Intro'

export default { 
    name: 'Home',
    components: {
      Intro,
  
    }
}
</script>

<style scoped>

.intro-bg {
  height: 800px;
  background-image: url("./../assets/soccer-field-3.jpg");
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
}

.intro {
  padding: 50px 15px;
  max-width: 1200px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
}

.img-fluid {
  width: 33%;
  padding: 70px 0;
  animation: fadein 5s;
  -moz-animation: fadein 5s;
  -webkit-animation: fadein 5s;
  -o-animation: fadein 5s;
  align-self: center; 
}

</style>