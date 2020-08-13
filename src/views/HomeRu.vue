<template>
    <section class="intro-bg">  
      <div class="intro">
        <intro-ru />
        <img class="img-fluid" src="./../assets/mocukup.png" alt="Pitch Match Mockup">
      </div>
    </section>
</template>

<script>
import IntroRu from './../components/IntroRu'

export default { 
    name: 'Home',
    components: {
      IntroRu,
  
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

@media screen and (max-width: 759px) {
  .intro {
    flex-direction: column;
    padding: 15px 15px;
    text-align: center;
    align-content: center;
    align-items: center;
  }
}
</style>