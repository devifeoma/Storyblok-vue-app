<template>
  <div v-editable="blok" >
    <div :key="blok._uid" v-for="blok in blok.columns" class="flex  px-6" >
      <component :blok="blok" :is="blok.component" />
    </div>
  </div>
</template>
 
<script setup>
const props = defineProps({
  blok: Object
});
</script>