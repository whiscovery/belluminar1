<template>
  <v-app>
    <v-main>
      <v-row justyfy="center">
        <v-col cols="12">
          <v-card elevation="1" class="mx-auto type1" max-width="450px">
            <v-img src="belluminar.PNG" height="200"></v-img>
            <v-form ref="form">
              <v-text-field
                v-model="name"
                label="Team name"
                required
              ></v-text-field>
              <v-text-field v-model="password" label="password" required>
              </v-text-field>
              <v-btn type="submit">submit</v-btn>
            </v-form>
          </v-card></v-col
        >
      </v-row>
    </v-main>
  </v-app>
</template>

<style>
.type1 {
  margin: 3% 10px 10px 10px;
  padding: 20px 20px 20px 20px;
}
</style>
