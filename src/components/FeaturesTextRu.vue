<template>
<div>
    <v-container
        v-for="align in alignments"
        :key="align"
        
    >
    <v-row class="header">
    <h1>
        Описание
    </h1>    
    </v-row>       
    <v-row class="p">
    <p>
        Pitch-Match - это новое приложение, удобноe и очень простоe в использовании. Получайте удовольствие от встречи с новыми людьми и игры в футбол!
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
        <h3>Бесплатная загрузка</h3>
        <p>Скачайте приложение совершенно бесплатно и сразу же его используйте</p>
        <img
          src="./../assets/soccer.svg" 
          alt="soccer icon"
          height="50"
          width="50" 
        />
        <h3>Играйте в футбол</h3>
        <p>Открывайте для себя все футбольные поля в городе и присоединяйтесь к реальным футбольным играм</p>
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
        <h3>Профиль игрока</h3>
        <p>Получайте оценки от других игроков и знакомьтесь с новыми людьми</p>
        <img
          src="./../assets/hearts.svg" 
          alt="free download"
          height="50"
          width="50" 
        />
        <h3>Создай свою игру</h3>
        <p>Забронируй близжайшее поле, создай свое футбольное событие и пригласи людей в свою игру</p>
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
  font-size: 24px;
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
  margin: 0 auto; 
  padding-top: 80px;
  padding-bottom: 10px;
  max-width: 700px;
  display: block;
}
</style>