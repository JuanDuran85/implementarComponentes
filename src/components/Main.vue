<template>
  <main class="mt-5">
      <JomboTron/>
      <Cards class="mt-5"/>
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
    }
}
</script>

<style>

</style>