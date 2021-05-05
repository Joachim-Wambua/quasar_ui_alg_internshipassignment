<template>
  <q-layout view="hHh lpR fFf">

    <q-header class="bg-white text-black">
      <q-toolbar class="logo">
        <q-toolbar-title >
          <q-avatar square>
            <img class="site_logo" src="../statics/proom_logo.png">
          </q-avatar>
        Proom
        </q-toolbar-title>

        <div class="menubar gt-sm">
          <q-tabs v-model="tab" no-caps class="tab-text" align="start">
            <q-route-tab to="/" label="Courses" />
            <q-route-tab to="/" label="Features" />
            <q-route-tab to="/" label="Support" />
            <q-btn dense round flat icon="email" class="email_button">
              <q-badge color="red" floating transparent >
                3
              </q-badge>
            </q-btn>
            <q-avatar class="profileavatar">
              <img src="../statics/profile_avatar.jpg">
            </q-avatar>
          </q-tabs>
      </div>

      <div class="lt-md">
        <q-btn flat 
          dense 
          round 
          @click="leftDrawerOpen=!leftDrawerOpen"
          icon = "menu" aria-label="Menu">
          
        </q-btn>
      </div>
      </q-toolbar>

      
    </q-header>

    <q-drawer
      v-model="leftDrawerOpen"
      bordered
      content-class="bg-grey-2"
    >
      <q-list>
        <q-item-label header>Menu</q-item-label>
        <q-item clickable tag="a" target="_blank" rel="noopener" href="">
          <q-item-section avatar>
            <q-icon name="school" />
          </q-item-section>
          <q-item-section>
            <q-item-label>Courses</q-item-label>
          </q-item-section>
        </q-item>
        <q-item clickable tag="a" target="_blank" rel="noopener" href="">
          <q-item-section avatar>
            <q-icon name="code" />
          </q-item-section>
          <q-item-section>
            <q-item-label>Features</q-item-label>
          </q-item-section>
        </q-item>
        <q-item clickable tag="a" target="_blank" rel="noopener" href="">
          <q-item-section avatar>
            <q-icon name="chat" />
          </q-item-section>
          <q-item-section>
            <q-item-label>Support</q-item-label>
          </q-item-section>
        </q-item>
      </q-list>
    </q-drawer>

    <q-page-container>
      <router-view />
    </q-page-container>

    <!-- <q-footer reveal elevated class="bg-grey-8 text-white">
      <q-toolbar>
        <q-toolbar-title>
          <q-avatar>
            <img src="https://cdn.quasar.dev/logo/svg/quasar-logo.svg">
          </q-avatar>
          Title
        </q-toolbar-title>
      </q-toolbar>
    </q-footer> -->

  </q-layout>
</template>

<script>
export default {
  data () {
    return {
      leftDrawerOpen: false
    }
  }
}
</script>

<style>

.logo{
  padding-left: 120px;
  font-family: Montserrat Black;
  size: 24px;
}

.tab-text{
  color: rgb(151, 151, 151);
  text-transform: lowercase;
  font-family: Montserrat-Medium;
}

.email_button{
 color: rgb(80, 80, 80);
 display: flex;
}

.menubar{
  padding-right: 120px;
  display: flex;
  align-self: center;
  justify-content: center;
  float: left;
  
}

.profileavatar{
  padding-left: 4px;
  size: 30px;

}

.site_logo{
  size: 18px;
  shape-outside: padding-box;
}

</style>