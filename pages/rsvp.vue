<template>
  <v-app>
    <v-container>
      <v-row>
        <v-col cols="12">
          <v-card>
            <v-card-title>RSVP</v-card-title>
            <v-card-subtitle>Please RSVP using the button below or using the paper insert and posting it back to us.</v-card-subtitle>
            <v-card-actions>
              <v-btn @click="goToForm" color="green lighten-3">RSVP here</v-btn>
            </v-card-actions>
          </v-card>
        </v-col>
      </v-row>
      <v-row>
        <v-col cols="12">
          <v-img max-height="800" src="/engadgement.jpg"></v-img>
        </v-col>
      </v-row>
    </v-container>
  </v-app>
</template>
<script>
  export default {
methods:{
  goToForm() {
      let url="https://forms.gle/kMmTiVxXnMv2CAdT8";
      window.open(url, '_blank').focus();
  }
}
}
</script>
<style>
.v-application {
  background-color: #fff176 !important
}

</style>
