<template>
   <div id="app">

        <app-Navbar></app-Navbar>
        <app-Home></app-Home>
        <app-Abt-Author></app-Abt-Author>
        <app-Creations></app-Creations>
        <app-Cast></app-Cast>
        <app-footer></app-footer> 
   


   </div>
   
</template>

<script>
  import navbar from "./cmp/navbar.vue";
  import home from "./cmp/home.vue";
  import abtAuthor from "./cmp/abtAuthor.vue";
  import creations from "./cmp/creation.vue";
  import cast from "./cmp/cast.vue";
  import footer from "./cmp/footer.vue";

  export default {
    components: {
      appNavbar : navbar,
      appHome : home,
      appAbtAuthor : abtAuthor,
      appCreations : creations,
      appCast : cast,
      appFooter : footer
    }
  }
</script>
