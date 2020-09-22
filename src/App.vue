<template>
  <ion-app>
    <ion-router-outlet />
    
  </ion-app>
</template>

<script lang="ts">
import { IonApp, IonRouterOutlet } from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
  name: 'App',
  components: {
    IonApp,
    IonRouterOutlet
  },
  data() {
    return{
      user: 'x',
      wtf: ''
    }
  },
  methods:{
    doTest(){
      //const a = Plugins.GoogleAuth.signIn({value: 'string'});
      
    },
    do2() {
      console.log(this)
      console.log(this.user);
    }

  }
});
</script>