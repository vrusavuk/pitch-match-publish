<template>
     <div>
        <h1>Pitch-Match</h1>
        <p>Soccer available for everyone at any time!</p>
            <div class="row">
              <div class="column">
                <a href="https://search.itunes.apple.com/WebObjects/MZContentLink.woa/wa/link?mt=8&path=appstore">
                  <img alt="App Store Badge" src="./../assets/app-store-badge.png"
                  width="200" height="auto">
                </a> 
              </div>
              <div class="column">
                <a href="https://play.google.com/store/apps?hl=en">
                  <img alt="App Store Badge" src="./../assets/google-play-badge.png"
                  width="200" height="auto">
                </a> 
              </div>
            </div>
          </div>
</template>

<script>
export default {
    name: 'IntroEnglish',
}
</script>

<style scoped>

.intro h1 {
  font-size: 80px;
  font-weight: bold;
  color: #01380d;
  margin-top: 180px;
  margin-bottom: 20px;
}

.intro p {
  font-size: 40px;
  font-weight: regular;
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

.column {
  float: left;
  width: 33.3%;
  
  
}

</style>