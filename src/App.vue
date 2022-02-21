<template>
    <v-app>
        <v-app-bar  app class="elevation-0">
            <v-app-bar-nav-icon @click="drawer = !drawer"></v-app-bar-nav-icon>
            <v-spacer></v-spacer>
            <v-app-bar-nav-icon @click="rightDrawer = !rightDrawer"></v-app-bar-nav-icon>
        </v-app-bar>

        <SideBar :drawer="drawer"/>
        <SideBarRight :rightDrawer="rightDrawer"/>

        <v-main>
            <router-view/>
        </v-main>
    </v-app>
</template>

<script>
import SideBar from './components/SideBar'
import SideBarRight from './components/SideBarRight'

export default {
    name: 'App',
    data: () => ({
        drawer: true,
        rightDrawer: true
    }),
    components: {
        SideBar,
        SideBarRight
    }
};
</script>
