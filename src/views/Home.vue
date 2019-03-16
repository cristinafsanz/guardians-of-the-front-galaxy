<template>
  <div class="home">
    <h1>My <strong>Videogames</strong> List</h1>
    <GamesList :games="games" />
  </div>
</template>

<script>
import GamesList from '@/components/GamesList.vue';

export default {
  name: 'Home',
  components: {
    GamesList,
  },
  data: () => ({
    games: [
      {
        id: 0,
        title: 'God of war',
        year: 2018,
        publish: new Date(2018, 11, 1),
        started: false,
        ended: false,
        percentage: 0,
        estimated: 20,
        score: 8,
        hype: 10,
        categories: ['Adventure', 'Vikings', 'One Player'],
        image: 'https://static.promodescuentos.com/pepperpdimages/threads/thread_large/default/251090_1.jpg',
      },
      {
        id: 1,
        title: 'The Witcher 3',
        year: 2015,
        publish: new Date(2018, 11, 1),
        started: true,
        ended: false,
        percentage: 0,
        estimated: 150,
        score: 9,
        hype: 10,
        categories: ['Open World', 'Rol', 'One Player'],
        image: 'https://lyricstranslate.com/files/styles/large/public/DVZUGpO.jpg',
      },
      {
        id: 2,
        title: 'Hellblade',
        year: 2017,
        publish: new Date(2018, 11, 1),
        started: false,
        ended: false,
        percentage: 0,
        estimated: 20,
        score: 7,
        hype: 7,
        categories: ['Adventure', 'One Player'],
        image: 'https://i11c.3djuegos.com/juegos/10125/proyecto_ninja_theory__nombre_temporal_/fotos/analisis/proyecto_ninja_theory__nombre_temporal_-4006254.jpg',
      },
      {
        id: 3,
        title: 'Skyrim',
        year: 2011,
        publish: new Date(2018, 11, 1),
        started: true,
        ended: false,
        percentage: 0,
        estimated: 100,
        score: 8,
        hype: 10,
        categories: ['Rol', 'One Player'],
        image: 'https://www.clavecd.es/wp-content/uploads/buy-the-elder-scrolls-5-skyrim-cd-key-pc-download-img1.jpg',
      },
    ],
  }),
};
</script>
