<template>
  <div id="app">
    <h1>Material UI</h1>
    <ul>
      <li><router-link to="/content">Content</router-link></li>
      <li><router-link to="/sample">Sample</router-link></li>
    </ul>
    <div class="view">
      <router-view></router-view>
    </div>
  </div>
</template>

<script>
  import Sample from './Sample.vue'
  import Content from './Content.vue'
  import VueRouter from 'vue-router'

  const router = new VueRouter({
    //mode:'history',
    routes:[
      {path:'/sample',component:Sample},
      {path:'/content',component:Content}
    ]
  });
  export default {
    name:'app',
    router
  }
</script>

<style>
  #app{margin:30px;}
  ul{list-style-type:none;margin:0;padding:0;overflow:hidden;background:#fff;}
  ul li{float:left;width:50%;}
  ul li a{display:block;padding:10px 0;text-align:center;font-size:18px;color:#000 !important;}
  ul li a:hover,.router-link-exact-active{background:#000;color:#fff !important;text-decoration:none !important;}
  .view{padding:30px 0;}
</style>
