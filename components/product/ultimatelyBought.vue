<template>
  <v-card flat class="white" width="100%">
    <v-card-title class="black--text">
      Customers who searched for {SKU} ultimately bought
    </v-card-title>
    <v-card-subtitle class="grey--text subtitle-2">Sponsored
      <v-icon color="grey" small>mdi-information</v-icon>
    </v-card-subtitle>
    <v-slide-group
      v-model="model"
      class="pa-4"
      show-arrows
    >
      <v-slide-item
        v-for="n in 15"
        :key="n"
        v-slot="{ active, toggle }"
      >
        <v-card
          :color="active ? undefined : 'grey lighten-1'"
          class="ma-4"
          height="200"
          width="100"
          @click="toggle"
        >
          <v-row
            class="fill-height"
            align="center"
            justify="center"
          >
            <v-scale-transition>
              <v-icon
                v-if="active"
                color="white"
                size="48"
                v-text="'mdi-close-circle-outline'"
              ></v-icon>
            </v-scale-transition>
          </v-row>
        </v-card>
      </v-slide-item>
    </v-slide-group>

    <v-divider class="background" />
  </v-card>
</template>

<script>
  export default {
    data: () => ({
      model: null,
    }),
  }
</script>