<template>
<div>
    <v-container
        v-for="align in alignments"
        :key="align"
        
    >
    <v-row class="header">
    <h1>
        Features
    </h1>    
    </v-row>       
    <v-row class="p">
    <p>
        Pitch-Match is a user friendly app and is very easy to use. We made sure you fully enjoy your experience, from meeting with people up to playing soccer!
    </p>    
    </v-row>
    <v-row class="pt">
      <v-col>
        <img
          src="./../assets/download.svg" 
          alt="download icon"
          height="50"
          width="50" 
        />
        <h3>Free download</h3>
        <p>You can freely download the app and use it right away</p>
        <img
          src="./../assets/soccer.svg" 
          alt="soccer icon"
          height="50"
          width="50" 
        />
        <h3>Play soccer</h3>
        <p>You can discover all soccer fields within your city and join real life soccer games</p>
      </v-col>
      <v-col>
        <div class="img-fluid"> 
          <mockup /> 
        </div>
      </v-col>
      <v-col>
       <img
          src="./../assets/profile.svg" 
          alt="profile icon"
          height="40"
          width="40" 
        />
        <h3>Player profile</h3>
        <p>Create a profile, receive ratings from other players and meet new people in your area</p>
        <img
          src="./../assets/hearts.svg" 
          alt="free download"
          height="50"
          width="50" 
        />
        <h3>Create games</h3>
        <p>Book a soccer filed nearby, create a game event and invite people to your game</p>
      </v-col>
    </v-row>
    </v-container>
  </div>
</template>

<script>
import Mockup from './../components/Mockup';
export default {
    name: 'FeaturesText',
    components: {
      Mockup
    },
    data: () => ({
      alignments: [
        'center',
    
      ],
    }),
    
}
</script>

<style scoped>

.header h1 {
  font-size: 45px;
  font-weight: bold;
  color: #01380d;
  max-width: 379px;
  line-height: 36px;
  padding: 25px;
  max-width: 500px;
  margin: 0 auto;
}

.p p {
  font-size: 25px;
  font-weight: 300;
  color: #291e33;
  max-width: 900px;
  line-height: 36px;
  padding: 0px;
  margin: 0 auto;
  text-align: center;
}

.pt h3 {
  font-size: 20px;
  font-weight: 500;
  color: #291e33;
  line-height: 36px;
  margin: 0 auto;
  text-align: center;
}

.pt p {
  font-size: 17px;
  font-weight: 300;
  color: #291e33;
  line-height: 25px;
  margin: 0 auto;
  text-align: center;
  max-width: 330px;
}

.col {
    display: column;
}

.text {
}

.img-fluid {
  justify-content: center;
  align-self: center;
  display: flex;
  padding: 0 !important;
}

.pt img {
  max-height: 600px;

  margin: 0 auto; /* poor attempt at centering */

  padding-top: 80px;
  padding-bottom: 10px;
  

  max-width: 700px;
  display: block;
}
</style>