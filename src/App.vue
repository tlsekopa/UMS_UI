<template>
  <div>
    <div>
      <a href="">SIGN-IN</a>
      <form-widget-vue @click="signInAction()"/>
    </div>
    <div>
      <a href="">SIGN-UP</a>
    </div>
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
import FormWidgetVue from './components/FormWidget.vue';

export default {
  name: 'App',
  components: {
    //HelloWorld,
    FormWidgetVue
     
  },
  data(){
    
  },
  methods: {
    signInAction(){
      
    }
  },
}
</script>

