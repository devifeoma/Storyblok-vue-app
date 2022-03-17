<template>
  <Suspense>
    <template #default>
      <Home />
    </template>
 
    <template #fallback>
      <div>Wait you App is Loading...</div>
    </template>
  </Suspense>
</template>


<script>
import Home from "./pages/Home.vue";

export default {
  name: "App",

  components: {
    Home,
  }
};
</script>