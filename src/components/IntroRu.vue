<template>
     <div>
        <h1>Pitch-Match</h1>
        <p>Футбол доступен для всех, в любое время!</p>
            <div class="row">
              <div class="c">
                <a href="https://apps.apple.com/ru/app/pitch-match/id1479033675">
                  <img alt="App Store Badge" src="./../assets/app-store-badge.png"
                  width="200" height="auto">
                </a> 
              </div>
              <div class="c">
                <router-link to="/ru">
                  <img alt="Google Play Badge" src="./../assets/google-play-badge.png"
                  width="200" height="auto">
                </router-link> 
              </div>
            </div>
      </div>
</template>

<script>
export default {
    name: 'IntroRu',
}
</script>

<style scoped>

.intro h1 {
  font-size: 85px;
  font-weight: 900;
  color: #01380d;
  margin-top: 180px;
  margin-bottom: 20px;
}

.intro p {
  font-size: 40px;
  font-weight: 600;
  color: #ffffff;
  max-width: 379px;
  line-height: 36px;
  margin-bottom: 36px;
  max-width: 500px;
  margin: 0 auto;
  margin-bottom: 50px;
}

.row {
  display: flex;
}

.row::after, .row::before {
  content: "";
  display: table;
  clear: both;
}

.c {
  float: left;
  width: 33.3%;
  position: relative;
  padding-left: 2.5%;  
}

@media screen and (max-width: 759px) {
  .intro h1 {
    font-size: 60px;
    font-weight: 900;
    margin-bottom: 10px;
    margin-top: 10px;
  }
  .intro p {
  font-size: 28px;
  font-weight: 600;
  
}
}
@media screen and (max-width: 759px) {

  .row {
    display: flex;
  }

  .c {
    width: 50%;
    align-self: center;
  }
  .c img {
    max-width: 250px;
  }
  .mockup {
    align-self: center;
  }
}
</style>