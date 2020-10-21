<template>
  <div class="container">
      <div class="row">
          <div v-for="item in dataCards" :key="item.id" class="col-12 col-sm-12 col-md-6 col-lg-4 col-xl-4">
            <div class="card">
                <img :src="item.urlImg" class="card-img-top" :alt="item.titulo">
                <div class="card-body">
                    <h5 class="card-title" v-text="item.titulo"></h5>
                    <p class="card-text" v-text="item.texto"></p>
                    <a :href="item.enlace" target="_blank" class="btn btn-primary" @click="visita">Ir al Sitio</a>
                </div>
            </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
    name: 'Cards',
    data() {
        return {
            contador: 0
        }
    },
    props: {
/*         urlImg: {
            type: String,
            required: true,
            default: "https://picsum.photos/seed/picsum/200/300"
        }, */
        dataCards: {
            type: Array,
            required: true
        }
    },
    methods: {
        visita(){
            this.contador++;
            this.$emit('contaVisita',this.contador);
        }
    }
}
</script>

<style>

</style>