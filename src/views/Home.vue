<template>
  <div class="home">
    <Navbar />
    <Best />
    <Create />
    <Platform />
    <Income />
    <Start />
    <Finish />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar.vue";
import Best from "@/components/Best.vue";
import Create from "@/components/Create.vue";
import Platform from "@/components/Platform.vue";
import Income from "@/components/Income.vue";
import Start from "@/components/Start.vue";
import Finish from "@/components/Finish.vue";

export default {
  name: "Home",
  components: {
    Navbar,
    Best,
    Create,
    Platform,
    Income,
    Start,
    Finish,
  },
};
</script>
