<template>
    <v-app theme="dark">
      <v-navigation-drawer
        v-model="drawer"
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
            :prepend-icon="item.icon"
            :title="item.title"
          />
        </v-list>
      </v-navigation-drawer>
      <v-app-bar
        fixed
        app
      >
        <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
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
        right: true,
        rightDrawer: false,
        title: "Sean's Portfolio"
      }
    }
  }
</script>
  