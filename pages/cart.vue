<template>
  <v-stepper
    v-model="e6"
    vertical
  >
    <v-stepper-step
      :complete="e6 > 1"
      editable
      step="1"
    >
      Cart

    </v-stepper-step>

    <v-stepper-content step="1" class="">


      <div>
        <vs-row class="mb-8">
          <vs-card type="2" class="mr-4  mb-4">
            <template #title>
              <h3>Pot with a plant</h3>
            </template>
            <template #img>
              <img src="https://vuesax.com/foto6.png" alt="">
            </template>
            <template #text>
              <p>
                Lorem ipsum dolor sit amet consectetur, adipisicing elit.
              </p>
            </template>
            <template #interactions>
              <vs-button danger icon>
                <v-icon v-text="'mdi-close-octagon'"></v-icon>

              </vs-button>
            </template>
          </vs-card>
          <vs-card type="2" class="mr-4 mb-4">
            <template #title>
              <h3>Pot with a plant</h3>
            </template>
            <template #img>
              <img src="https://vuesax.com/foto6.png" alt="">
            </template>
            <template #text>
              <p>
                Lorem ipsum dolor sit amet consectetur, adipisicing elit.
              </p>
            </template>
            <template #interactions>
              <vs-button danger icon>
                <v-icon v-text="'mdi-close-octagon'"></v-icon>

              </vs-button>
            </template>
          </vs-card>
          <vs-card type="2" class="mr-4 mb-4">
            <template #title>
              <h3>Pot with a plant</h3>
            </template>
            <template #img>
              <img src="https://vuesax.com/foto6.png" alt="">
            </template>
            <template #text>
              <p>
                Lorem ipsum dolor sit amet consectetur, adipisicing elit.
              </p>
            </template>
            <template #interactions>
              <vs-button danger icon>
                <v-icon v-text="'mdi-close-octagon'"></v-icon>

              </vs-button>
            </template>
          </vs-card>
        </vs-row>
      </div>







      <v-btn
        color="primary"
        @click="e6 = 2"
      >
        Continue
      </v-btn>
    </v-stepper-content>

    <v-stepper-step
      :complete="e6 > 2"

      step="2"
    >
      Payment
    </v-stepper-step>

    <v-stepper-content step="2">


      <div>
        <vs-row :w="12">
        <vs-button>
          <template  >
            <v-icon class="mr-3" v-text="'mdi-credit-card'"></v-icon>
          </template>
          Credit Card
        </vs-button>
        <vs-button
          warn
          gradient
        >
          Paypal
        </vs-button>
        </vs-row>
      </div>

      <v-card
        color="grey lighten-1"
        class="mb-12"
        height="200px"
      ></v-card>


    </v-stepper-content>


  </v-stepper>
</template>

<script>
export default {
  name: "cart",
  data () {
    return {
      e6: 1,
    }
  },
}
</script>

<style scoped>

</style>
