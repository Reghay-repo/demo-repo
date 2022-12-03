<template>
<v-row>
  <v-col cols="8" >
           <v-text-field
               density="compact"
               class="rounded-lg"
               variant="outlined"
               placeholder="search for something"
                prepend-inner-icon="mdi-magnify"
          ></v-text-field>
  </v-col>
</v-row>
</template>


<script setup>
  const model = ref(null)
</script>

<style scoped>
</style>