<template>
<v-row align="center">
  <v-col>
    <v-card class="mx-auto px-6 py-8" max-width="500" elevation="3" >
         <v-img
             class="mx-auto"
             width="200"
             height="200"
      src="logo.png"
      cover
    ></v-img>
        <v-text-field
                v-model="email"
                variant="outlined"
                class="mb-2"
                clearable
                label="Email"
              ></v-text-field>
      <v-text-field
                v-model="password"
                variant="outlined"
                class="mb-2"
                clearable
                label="password"
                type="password"
              ></v-text-field>


        <br>
        <v-btn
          block
          color="primary"
          size="large"
          :loading="loading"
          type="submit"
          @click="login"
        >
          Sign In
        </v-btn>
  </v-card>
  </v-col>
</v-row>
</template>

<script setup>
const router = useRouter()
definePageMeta({
  layout: "default",
});
const email =ref('')
const password =ref('')
const loading =ref(false)

const login = () => {
    // login dyal login
    loading.value = true
    setTimeout(() => {

    loading.value = false
    router.push({path:'/'})
    },1000)
}


</script>

<style scoped>

</style>