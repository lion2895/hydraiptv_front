<template>
  <v-stepper class=""
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

    <v-stepper-content step="1" class="pl-1">


      <div>
        <vs-row :w="12" class="mb-5" justify="center">
          <vs-card type="4" class="mr-4  mb-4">
            <template #title>
              <vs-row class="mb-3" :w="12">
                <vs-col :w="7">
                  <h3>44.95 EUR</h3>
                </vs-col>
                <vs-col :w="5"> <vs-switch  color="#ff448a"  v-model="adultestate" >
                  <template #off>
                    No Adult
                  </template>
                  <template #on>
                    with Adult
                  </template>
                </vs-switch></vs-col>
              </vs-row>



            </template>
            <template #img>

              <img src="https://vuesax.com/foto6.png" alt="">


            </template>
            <template #text >
              <vs-row :w="12" align="center">
                <vs-col :w="4">
                   Devices
                </vs-col>
                <vs-col class="mb-3" :w="8">
                  <vs-select   placeholder="Select a Device" v-model="selectvalue">
                    <vs-option label="Vuesax" value="1">
                      Vuesax
                    </vs-option>
                    <vs-option label="Vue" value="2">
                      Vue
                    </vs-option>
                    <vs-option label="Javascript" value="3">
                      Javascript
                    </vs-option>
                    <vs-option disabled label="Sass" value="4">
                      Sass
                    </vs-option>
                    <vs-option label="Typescript" value="5">
                      Typescript
                    </vs-option>
                    <vs-option label="Webpack" value="6">
                      Webpack
                    </vs-option>
                    <vs-option label="Nodejs" value="7">
                      Nodejs
                    </vs-option>
                  </vs-select>
                </vs-col>
                <vs-col :w="4">
                    Quantity
                </vs-col>
                <vs-col   :w="6" align="center">
                  <vs-input
                    primary

                    type="number"

                    placeholder="Quantity" />

                </vs-col>


              </vs-row>





            </template>







            <template #interactions style="width: -webkit-fill-available;">

              <vs-button danger icon>
                <v-icon v-text="'mdi-close-octagon'"></v-icon>
              </vs-button>
              <vs-button class="btn-chat" shadow primary>

                <span class="span">
          12 month
        </span>
              </vs-button>











            </template>

          </vs-card>
          <vs-card type="4" class="mr-4  mb-4">
            <template #title>
              <vs-row class="mb-3" :w="12">
                <vs-col :w="7">
                  <h3>44.95 EUR</h3>
                </vs-col>
                <vs-col :w="5"> <vs-switch  color="#ff448a"  v-model="adultestate" >
                  <template #off>
                    No Adult
                  </template>
                  <template #on>
                    with Adult
                  </template>
                </vs-switch></vs-col>
              </vs-row>



            </template>
            <template #img>

              <img src="https://vuesax.com/foto6.png" alt="">


            </template>
            <template #text >
              <vs-row :w="12" align="center">
                <vs-col :w="4">
                  Devices
                </vs-col>
                <vs-col class="mb-3" :w="8">
                  <vs-select   placeholder="Select a Device" v-model="selectvalue">
                    <vs-option label="Vuesax" value="1">
                      Vuesax
                    </vs-option>
                    <vs-option label="Vue" value="2">
                      Vue
                    </vs-option>
                    <vs-option label="Javascript" value="3">
                      Javascript
                    </vs-option>
                    <vs-option disabled label="Sass" value="4">
                      Sass
                    </vs-option>
                    <vs-option label="Typescript" value="5">
                      Typescript
                    </vs-option>
                    <vs-option label="Webpack" value="6">
                      Webpack
                    </vs-option>
                    <vs-option label="Nodejs" value="7">
                      Nodejs
                    </vs-option>
                  </vs-select>
                </vs-col>
                <vs-col :w="4">
                  Quantity
                </vs-col>
                <vs-col   :w="6" align="center">
                  <vs-input
                    primary

                    type="number"

                    placeholder="" />

                </vs-col>


              </vs-row>





            </template>







            <template #interactions style="width: -webkit-fill-available;">

              <vs-button danger icon>
                <v-icon v-text="'mdi-close-octagon'"></v-icon>
              </vs-button>
              <vs-button class="btn-chat" shadow primary>

                <span class="span">
          12 month
        </span>
              </vs-button>











            </template>

          </vs-card>
          <vs-card type="4" class="mr-4  mb-4">
            <template #title>
              <vs-row class="mb-3" :w="12">
                <vs-col :w="7">
                  <h3>44.95 EUR</h3>
                </vs-col>
                <vs-col :w="5"> <vs-switch  color="#ff448a"  v-model="adultestate" >
                  <template #off>
                    No Adult
                  </template>
                  <template #on>
                    with Adult
                  </template>
                </vs-switch></vs-col>
              </vs-row>



            </template>
            <template #img>

              <img src="https://vuesax.com/foto6.png" alt="">


            </template>
            <template #text >
              <vs-row :w="12" align="center">
                <vs-col :w="4">
                  Devices
                </vs-col>
                <vs-col class="mb-3" :w="8">
                  <vs-select   placeholder="Select a Device" v-model="selectvalue">
                    <vs-option label="Vuesax" value="1">
                      Vuesax
                    </vs-option>
                    <vs-option label="Vue" value="2">
                      Vue
                    </vs-option>
                    <vs-option label="Javascript" value="3">
                      Javascript
                    </vs-option>
                    <vs-option disabled label="Sass" value="4">
                      Sass
                    </vs-option>
                    <vs-option label="Typescript" value="5">
                      Typescript
                    </vs-option>
                    <vs-option label="Webpack" value="6">
                      Webpack
                    </vs-option>
                    <vs-option label="Nodejs" value="7">
                      Nodejs
                    </vs-option>
                  </vs-select>
                </vs-col>
                <vs-col :w="4">
                  Quantity
                </vs-col>
                <vs-col   :w="6" align="center">
                  <vs-input
                    primary

                    type="number"

                     />

                </vs-col>


              </vs-row>





            </template>







            <template #interactions style="width: -webkit-fill-available;">

              <vs-button danger icon>
                <v-icon v-text="'mdi-close-octagon'"></v-icon>
              </vs-button>
              <vs-button class="btn-chat" shadow primary>

                <span class="span">
          12 month
        </span>
              </vs-button>











            </template>

          </vs-card>


        </vs-row>

          <v-simple-table class="mb-8 mr-4">
            <template v-slot:default>
              <thead>
              <tr>
                <th class="text-left">
                  TOTAL
                </th>
                <th class="text-right" >
                  22.5 EUR
                </th>
              </tr>
              </thead>
            </template>
          </v-simple-table>

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
      selectvalue:0,
      adultestate : false
    }
  },
}
</script>

<style scoped>

</style>
