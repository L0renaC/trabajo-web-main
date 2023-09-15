<template>
  <v-card
    class="mx-auto"
    width="400"
  >
  <div>
    <center>
      <h1>Login</h1>
      <p>Esta es una aplicación que permite gestionar las tareas de los estudiantes</p>
        <v-sheet width="300" class="mx-auto">
    <v-card-item>
    <v-form fast-fail @submit.prevent>

      <v-text-field
        v-model="Email"
        label="Email"
        :rules="Email"
      ></v-text-field>

       <v-text-field
        label="Password"
        type="Password"
        hint="Password"
      ></v-text-field>
      

      <v-btn href="/tareas" type="submit" block class="mt-2">Ingresar</v-btn>
    </v-form>
    </v-card-item>
  </v-sheet>

<br>
<br>
      <NuxtLink to="/tareas">
        Click para iniciar (Con nuxtLink)
      </NuxtLink>
    </center>

  </div>
  </v-card>
</template>
<script>
definePageMeta({
  layout: "blank",
});
</script>