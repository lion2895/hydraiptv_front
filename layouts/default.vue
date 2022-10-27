<template>
  <v-app >
    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
    >
      <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-app-bar
      :clipped-left="clipped"
      fixed
      app
    >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <v-btn
        icon
        @click.stop="miniVariant = !miniVariant"
      >
        <v-icon>mdi-{{ `chevron-${miniVariant ? 'right' : 'left'}` }}</v-icon>
      </v-btn>
      <v-toolbar-title>{{ title }}</v-toolbar-title>
      <v-spacer />


      <v-btn
        class="mr-8"
        depressed
        icon

      >
        <v-badge class="mt-2"
                 :content="5"
                 :value="5"
                 bordered
                 color="green"


        >
        <v-icon class="">mdi-cart</v-icon>
        </v-badge>
      </v-btn>


      <v-menu offset-y transition="slide-y-transition" max-width="300">
        <template v-slot:activator="{ on, attrs }">

            <vs-avatar color="#7d33ff"  v-bind="attrs"
                       v-on="on">
              <template #text >
                Ayoub MArgoum
              </template>
            </vs-avatar>


        </template>
        <v-list>
          <v-list-item-group>
          <v-list-item>
            <v-list-item-icon class="mr-1 ml-0 pr-0">
              <v-icon class="" v-text="icon"></v-icon>
            </v-list-item-icon>
            <v-list-item-content>
            <v-list-item-title>Profile</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          <v-list-item>
            <v-list-item-icon class="mr-1 mr-1 ml-0 pr-0">
              <v-icon class="" v-text="'mdi-logout'"></v-icon>
            </v-list-item-icon>
            <v-list-item-content>
            <v-list-item-title>Log out</v-list-item-title>
            </v-list-item-content>
          </v-list-item>
          </v-list-item-group>
        </v-list>
      </v-menu>



    </v-app-bar>
    <v-main>
      <v-container>
        <Nuxt />
      </v-container>
    </v-main>
    <v-footer
      :absolute="!fixed"
      app
    >
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  name: 'DefaultLayout',
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-cart',
          title: 'My Cart',
          to: '/cart'
        },
        {
          icon: 'mdi-order-bool-descending',
          title: 'My Orders',
          to: '/orders'
        },
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'HYDRA IPTV',
      icon :'mdi-account'
    }
  }
}
</script>
