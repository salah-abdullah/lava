<template>
  <v-card>
    <v-layout>
      <v-navigation-drawer
        expand-on-hover
        rail
      >
        <v-list>
          <v-list-item
            prepend-icon="mdi-account"
            title="account"
          />
        </v-list>

        <v-divider />

        <v-list
          density="compact"
          nav
        >
          <v-list-item
            prepend-icon="mdi-folder"
            title="My Files"
            value="myfiles"
          />

          <v-list-item
            prepend-icon="mdi-account-multiple"
            title="Shared with me"
            value="shared"
          />

          <v-list-item
            prepend-icon="mdi-star"
            title="Starred"
            value="starred"
          />
        </v-list>
      </v-navigation-drawer>

      <v-main style="height:100em" />
    </v-layout>
  </v-card>
</template>
<script setup lang="ts">
</script>
