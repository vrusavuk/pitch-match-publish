<template>
<section>
    <section class="features-bg">  
      <div class="features">
        <v-row justify="space-around">
            <v-chip-group
            multiple
            active-class="white"
            dark
            >
            <v-chip v-for="tag in tags" :key="tag">
                {{ tag }}
            </v-chip>
            </v-chip-group>
    </v-row>  
      </div>
    </section>
    <section class="bg-container">
    <div>

        <features-text-ru />

    </div>
    </section>
</section>  
</template>

<script>
import Mockup from './../components/Mockup';
import FeaturesTextRu from './../components/FeaturesTextRu';


export default {
    name: 'FeaturesRu',
    components: {
        Mockup,
        FeaturesTextRu,
    },
    data: () => ({
      tags: [
        'Играй в футбол',
        'Создавай игры',
        'Присоединяйся к играм',
        'Бронируй поле поблизости',
        'Лента событий',
        'Профиль',
        'Оценивай игру',
      ],
    }),
}
</script>

<style scoped>

.features-bg {
  height: 150px;
  background: linear-gradient(36.1deg, #42cbf7 0%, #4a098d 100%);
}

.features {
  padding: 50px 15px;
  max-width: 1200px;
  margin: 0 auto;
  display: flex;
  justify-content: space-between;
}

.bg-container {
    height: 800px;
    width: 100%;
    background: linear-gradient(180deg, #ebecee 0%, #c7c2cc 100%);
}
</style>