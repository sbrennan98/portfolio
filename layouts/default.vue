<template>
    <v-app theme="dark">
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
            <v-list-item-title v-text="item.title" />
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
        <v-btn
          icon
          @click.stop="clipped = !clipped"
        >
          <v-icon>mdi-application</v-icon>
        </v-btn>
        <v-toolbar-title v-text="title" />
      </v-app-bar>
      <v-main>
        <v-container>
          <slot />
        </v-container>
      </v-main>
      <v-footer
        :absolute="!fixed"
        app
      >
        <SeanFooter />
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
        fixed: true,
        items: [
          {
            icon: 'mdi-home',
            title: 'Homepage',
            to: '/'
          },
          {
            icon: 'mdi-account',
            title: 'Bio',
            to: '/sean'
          },
          {
            icon: 'mdi-chart-bubble',
            title: 'Inspire',
            to: '/sean/inspire'
          },
          {
            icon: 'mdi-apps',
            title: 'Projects',
            to: '/sean/projects'
          }
        ],
        miniVariant: false,
        right: true,
        rightDrawer: false,
        title: "Sean's Portfolio"
      }
    }
  }
</script>
  