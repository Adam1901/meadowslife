<template>
  <div>
   <h1>Numbers of days until the magical day {{ daysUntil }}</h1>
  </div>
</template>

<script>
export default {
  name: "countdown",
  data: function () {
    return {
      daysUntil: 0
    }
  },
  mounted() {
    const oneDay = 24 * 60 * 60 * 1000; // hours*minutes*seconds*milliseconds
    const wedding = new Date(2022, 2, 19);
    const now = new Date();
    this.daysUntil = Math.round(Math.abs((now - wedding) / oneDay));
  }
}
</script>

<style scoped>

</style>
