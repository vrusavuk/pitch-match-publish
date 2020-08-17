<template>
     <div>
        <h1>Pitch-Match</h1>
        <p>Soccer available for everyone at any time!</p>
            <div class="row">
              <div class="c">
                <router-link to="/en">
                  <img alt="App Store Badge" src="./../assets/app-store-badge.png"
                  width="200" height="auto">
                </router-link> 
              </div>
              <div class="c">
                <router-link to="/en">
                  <img alt="App Store Badge" src="./../assets/google-play-badge.png"
                  width="200" height="auto">
                </router-link> 
              </div>
            </div>
          </div>
</template>

<script>
export default {
    name: 'Intro',
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

</style>