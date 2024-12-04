<template>
  <div class="text-center pa-4">
    <v-dialog
      v-model="dialog"
      max-width="400"
      persistent
    >
      <template v-slot:activator="{ props: activatorProps }">
  
        <v-icon v-bind="activatorProps" icon="mdi-logout"></v-icon>

      </template>

      <v-card
        prepend-icon="mdi-logout"
        text="Are you sure?"
        title="LOG OUT"
      >
        <template v-slot:actions>
          <v-spacer></v-spacer>

          <v-btn @click="dialog = false">
            cancel
          </v-btn>

          <v-btn @click="dialog = false">
            Log out
          </v-btn>
        </template>
      </v-card>
    </v-dialog>
  </div>
</template>
<script>
  export default {
    data () {
      return {
        dialog: false,
      }
    },
  }
</script>