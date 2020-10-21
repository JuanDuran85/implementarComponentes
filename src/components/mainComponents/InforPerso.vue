<template>
  <div class="imgFondo">
      <div v-for="(item, index) in datosRyM" :key="index">
          <img :src="item.image" :alt="item.name" @click="$emit('clicrm', index)"> <span>{{item.name}}</span>
      </div>
  </div>
</template>

<script>
export default {
    name: 'InfoPerso',
    props: {
        datosRyM: {
            type: Array,
            required: true
        }
    }
}
</script>

<style scoped>
    .imgFondo {
        background-image: url('../../assets/cropped-RM_page-header_background1-3.png');
        background-size: cover;
    }
    img {
        border-radius: 50%;
        width: 120px;
    }
    span {
        color: green;
        font-size: 24px;
        font-weight: 700;
    }
</style>