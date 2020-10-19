<template>
  <main class="mt-5">
      <JomboTron/>
      <Cards class="mt-5" :dataCards="dataVarios"/>
  </main>
</template>

<script>
import JomboTron from './mainComponents/JumboTron.vue';
import Cards from './mainComponents/Cards.vue';

export default {
    name: 'Main',
    components: {
        JomboTron,
        Cards
    },
    data() {
        return {
           /*  url: 'https://picsum.photos/id/237/200/300'  */  
           dataVarios: [
                {urlImg: 'https://picsum.photos/id/237/200/300', id: '1', texto: 'Lorem ipsum dolor sit amet consectetur adipisicing elit.', enlace: 'https://es.wikipedia.org/wiki/Portal:Perros'},
                {urlImg: 'https://picsum.photos/seed/picsum/200/300', id: '2', texto: 'Illo commodi modi ullam mollitia sapiente provident debitis consequatur quasi nesciunt voluptatibus.', enlace: 'https://es.wikipedia.org/wiki/Monta%C3%B1a'},
                {urlImg: 'https://picsum.photos/id/237/200/300', id: '3', texto: 'Lorem ipsum dolor sit amet consectetur adipisicing elit.', enlace: 'https://es.wikipedia.org/wiki/Portal:Perros'},
                {urlImg: 'https://picsum.photos/seed/picsum/200/300', id: '4', texto: 'Illo commodi modi ullam mollitia sapiente provident debitis consequatur quasi nesciunt voluptatibus.', enlace: 'https://es.wikipedia.org/wiki/Monta%C3%B1a'},
                {urlImg: 'https://picsum.photos/id/237/200/300', id: '5', texto: 'Lorem ipsum dolor sit amet consectetur adipisicing elit.', enlace: 'https://es.wikipedia.org/wiki/Portal:Perros'},
                {urlImg: 'https://picsum.photos/seed/picsum/200/300', id: '6', texto: 'Illo commodi modi ullam mollitia sapiente provident debitis consequatur quasi nesciunt voluptatibus.', enlace: 'https://es.wikipedia.org/wiki/Monta%C3%B1a'}
           ]   
        }
    },
}
</script>

<style>

</style>