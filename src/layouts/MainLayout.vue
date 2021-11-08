<template>
  <q-layout view="lHh Lpr lFf">
   <q-header
      class="bg-white text-grey-10"
      bordered>
      <q-toolbar class="toolbar-size constrain">
        <q-btn 
         class="large-screen-only q-mr-xs"
          icon="eva-camera-outline"
          size="18px"
          to="/camera"
          flat
          round
          dense
           />
           <q-separator class="large-screen-only"
             vertical
             spaced />
        <q-toolbar-title class="text-grand-hotel text-bold toolbar-title">
          Quasargra
        </q-toolbar-title>
        <q-btn 
         class="large-screen-only"
          icon="eva-home-outline"
          size="18px"
          to="/"
          flat
          round
          dense
           />
        
      </q-toolbar>
    </q-header>
   <q-footer class="bg-white small-screen-only" bordered>
    <q-tabs
      class="text-grey-10"
      active-color="primary"
      indicator-color="transparent">
        <q-route-tab
          to="/"
          name="home"
          icon="eva-home-outline"
          />
        <q-route-tab
          to="/camera"
          name="camera"
          icon="eva-camera-outline"
           />
      
      </q-tabs>
       
      </q-footer>

    <q-page-container class="bg-grey-1">
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>

</script>

<style lang="sass">
 .q-toolbar__title
   font-size: 30px
 .q-footer
   .q-tab__icon
     font-size: 30px   
</style>