<template>
   <v-list-group :value="items.title">
        <template v-slot:activator="{ props }">
          <v-list-item
            v-bind="props"
            prepend-icon="mdi-circle"
            :title="items.title"
          ></v-list-item>
        </template>

          <v-list-item
              dense
              v-for="(title, i) in items.list"
              :key="i"
              :title="title"
              :value="title"
          ></v-list-item>
      </v-list-group>
</template>

<script setup>
defineProps({
  items:{
    title:String,
    list:Array
  }
})
</script>

<style scoped>

</style>