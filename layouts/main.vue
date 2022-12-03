<template>
  <v-app id="inspire"  v-if="!loading">
    <v-navigation-drawer
          app
          v-model="drawer"
          permanent
        >
          <v-list-item
            title="Web app"
          >
          </v-list-item>
          <DrawerList />
        </v-navigation-drawer>

    <v-app-bar density="compact" >
      <v-app-bar-nav-icon @click="drawer = !drawer "></v-app-bar-nav-icon>
<!--         <v-spacer></v-spacer>-->
<!--    search bar    -->
        <SearchBar class="mt-2" />
<!--    notifications    -->
      <Notifications  class="mr-4 ma-2"/>
      <Avatar class="mx-4"></Avatar>

    </v-app-bar>

    <v-main >
      <slot></slot>
    </v-main>
  </v-app>
</template>

<script setup >
const drawer = ref(true)
const rail = ref(true)
const loading = ref(true)

onMounted(() => {
  loading.value = false
})

</script>
