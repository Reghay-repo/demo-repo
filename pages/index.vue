<template>
  <div>
    <h4>Hello modification</h4>
  </div>
  <div>
    <h4>Hello modifications from oussama</h4>
    <h4>another Hello modifications from oussama</h4>

  </div>

  <div>
    <h6>text by saad</h6>

<div>modification by osm from webstorm</div>
<div>modification by osm from webstorm 2</div>
    jhkjkjhkjhkjhkjhkjhkjhkjhkjh
  </div>
  <v-form>
    <v-container>
      <v-row>
        <v-col cols="12" sm="6" md="4">
          <v-text-field dense label="Regular"></v-text-field>
        </v-col>

        <v-col cols="12" sm="6" md="4">
          <v-text-field class="rounded-pill" style="border-radius: 100px"></v-text-field>
        </v-col>

        <v-col cols="12" sm="6" md="4">
          <v-text-field label="Filled" placeholder="Dense & Rounded" filled rounded dense></v-text-field>
        </v-col>

        <v-col cols="12" sm="6" md="4">
          <v-text-field label="Solo" solo dense></v-text-field>
        </v-col>

        <v-col cols="12" sm="6" md="4">
          <v-text-field label="Outlined" outlined dense></v-text-field>
        </v-col>

        <v-col cols="12" sm="6" md="4">
          <v-text-field label="Outlined" placeholder="Placeholder" outlined dense></v-text-field>
        </v-col>
      </v-row>
    </v-container>
  </v-form>
</template>

<script setup>
// // This will work in both `<script setup>` and `<script>`
definePageMeta({
  layout: "main",
});
</script>

<style scoped>

</style>