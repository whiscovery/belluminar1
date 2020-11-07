<template>
  <v-main>
    <v-container>
      <v-row>
        <template v-for="(category, n) in categories">
          <v-col :key="n" class="mt-2" cols="12">
            <strong>{{ category }}</strong>
          </v-col>

          <v-col v-for="j in 6" :key="`${n}${j}`" cols="6" md="2">
            <v-sheet height="200" width="180" elevation="1" rounded="xl">{{
              j
            }}</v-sheet>
          </v-col>
        </template>
      </v-row>
    </v-container>
  </v-main>
</template>
<script>
export default {
  data: () => ({
    categories: ["Web", "Pwnable", "MISC"]
  })
};
</script>
