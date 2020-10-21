<template>
  <main class="mt-5">
    <div v-if="conteo > 0" class="alert alert-success" role="alert">
       Clic N°: {{conteo}}.
    </div>
    <div v-else class="alert alert-light" role="alert">
        No hay clic aun...
    </div>
    <JomboTron/>
    <Cards class="mt-5" :dataCards="dataVarios" @contaVisita="mostrarVisita"/>
    <hr>
    <info-perso :datosRyM="datosRyM"></info-perso>
  </main>
</template>

<script>
import JomboTron from './mainComponents/JumboTron.vue';
import Cards from './mainComponents/Cards.vue';
import InfoPerso from './mainComponents/InforPerso.vue';

export default {
    name: 'Main',
    components: {
        JomboTron,
        Cards,
        InfoPerso
    },
    methods: {
        mostrarVisita(valor){
            this.conteo = valor;
        }
    },
    data() {
        return {
            conteo: 0,
           /*  url: 'https://picsum.photos/id/237/200/300'  */  
            dataVarios: [
                {urlImg: 'https://picsum.photos/id/237/200/300', id: '1', texto: 'Lorem ipsum dolor sit amet consectetur adipisicing elit.', enlace: 'https://es.wikipedia.org/wiki/Portal:Perros', titulo: "Tarjeta numero 1"},
                {urlImg: 'https://picsum.photos/seed/picsum/200/300', id: '2', texto: 'Illo commodi modi ullam mollitia sapiente provident debitis consequatur quasi nesciunt voluptatibus.', enlace: 'https://es.wikipedia.org/wiki/Monta%C3%B1a', titulo: "Tarjeta numero 2"},
                {urlImg: 'https://picsum.photos/id/237/200/300', id: '3', texto: 'Lorem ipsum dolor sit amet consectetur adipisicing elit.', enlace: 'https://es.wikipedia.org/wiki/Portal:Perros', titulo: "Tarjeta numero 3"},
                {urlImg: 'https://picsum.photos/seed/picsum/200/300', id: '4', texto: 'Illo commodi modi ullam mollitia sapiente provident debitis consequatur quasi nesciunt voluptatibus.', enlace: 'https://es.wikipedia.org/wiki/Monta%C3%B1a', titulo: "Tarjeta numero 4"},
                {urlImg: 'https://picsum.photos/id/237/200/300', id: '5', texto: 'Lorem ipsum dolor sit amet consectetur adipisicing elit.', enlace: 'https://es.wikipedia.org/wiki/Portal:Perros', titulo: "Tarjeta numero 5"},
                {urlImg: 'https://picsum.photos/seed/picsum/200/300', id: '6', texto: 'Illo commodi modi ullam mollitia sapiente provident debitis consequatur quasi nesciunt voluptatibus.', enlace: 'https://es.wikipedia.org/wiki/Monta%C3%B1a', titulo: "Tarjeta numero 6"}
            ],
            datosRyM: [
                {name: "Rick Sanchez", image: "https://rickandmortyapi.com/api/character/avatar/1.jpeg"},
                {name: "Morty Smith", image: "https://rickandmortyapi.com/api/character/avatar/2.jpeg"},
                {name: "Summer Smith", image: "https://rickandmortyapi.com/api/character/avatar/3.jpeg"},
                {name: "Beth Smith", image: "https://rickandmortyapi.com/api/character/avatar/4.jpeg"},
                {name: "Jerry Smith", image: "https://rickandmortyapi.com/api/character/avatar/5.jpeg"},
            ]  
        }
    },
}
</script>

<style>

</style>