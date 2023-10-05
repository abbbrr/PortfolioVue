<script>  
  import Navbar from "@/components/Navbar.vue";
  import Main from "@/components/Main.vue";
  import Header from "@/components/Header.vue";
  import LanguageCard from "@/components/LanguageCard.vue";


  export default {
  name: "App",
  components: {
    LanguageCard,
    Navbar,
    Main,
    Header,
  },
};
</script>

<template>
 <div id = "app">
    <Navbar /> 
     <Main />
    <Header />
    <LanguageCard />
 </div>
</template>

<style >
@import "@/styles.css";

</style>
