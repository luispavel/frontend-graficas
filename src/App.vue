<template>
  <v-app>
    <v-main>
      <group-chart/>
    </v-main>
  </v-app>
</template>

<script>
import GroupChart from './components/Chart/GroupChart.vue'
export default {
  name: 'App',

  data: () => ({
    //
  }),
  components: {
    GroupChart
  }
};
</script>
