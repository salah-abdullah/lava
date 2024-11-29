<template>
  <v-card>
    <v-layout>
      <v-navigation-drawer
        v-model="drawer"
        :rail="rail"
        permanent
        @click="rail = false"
      >
        <v-list-item
          prepend-icon="mdi-home-city"
          title="Lava"
          nav
        >
          <template #append>
            <v-btn
              icon="mdi-chevron-left"
              variant="text"
              @click.stop="rail = !rail"
            />
          </template>
        </v-list-item>

        <v-divider />

        <v-list
          density="compact"
          nav
        >
          <v-list-item
            prepend-icon="mdi-home-city"
            title="Home"
            value="home"
          />

          <v-list-item
            prepend-icon="mdi-account"
            title="My Account"
            value="account"
          />

          <v-list-item
            prepend-icon="mdi-account-group-outline"
            title="Users"
            value="users"
          />

        </v-list>
      </v-navigation-drawer>
      <v-main style="height: 250px" />
    </v-layout>
  </v-card>
</template>
<script>
export default {
  data () {
    return {
      drawer: true,
      rail: true,
    }
  },
}
</script>
