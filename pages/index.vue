<template>
  <div><h4>Hello modification</h4></div>
  <div><p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Amet animi debitis eaque est iste natus quos tenetur! Blanditiis corporis dolorem impedit, ipsam itaque quod reprehenderit. Consequuntur eum mollitia quibusdam rem?</p></div>
  <v-form>
    <v-container>
      <v-row>
        <v-col
          cols="12"
          sm="6"
          md="4"
        >
          <v-text-field
            dense
            label="Regular"
          ></v-text-field>
        </v-col>

        <v-col
          cols="12"
          sm="6"
          md="4"
        >
          <v-text-field
         class="rounded-pill"
         style="border-radius: 100px"
          ></v-text-field>
        </v-col>

        <v-col
          cols="12"
          sm="6"
          md="4"
        >
          <v-text-field
            label="Filled"
            placeholder="Dense & Rounded"
            filled
            rounded
            dense
          ></v-text-field>
        </v-col>

        <v-col
          cols="12"
          sm="6"
          md="4"
        >
          <v-text-field
            label="Solo"
            solo
            dense
          ></v-text-field>
        </v-col>

        <v-col
          cols="12"
          sm="6"
          md="4"
        >
          <v-text-field
            label="Outlined"
            outlined
            dense
          ></v-text-field>
        </v-col>

        <v-col
          cols="12"
          sm="6"
          md="4"
        >
          <v-text-field
            label="Outlined"
            placeholder="Placeholder"
            outlined
            dense
          ></v-text-field>
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