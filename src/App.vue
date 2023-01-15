<template>
 <div class="overflow-hidden">
  <NavbarMenu></NavbarMenu>
  <Info_detail></Info_detail>
  <Education_info></Education_info>
   <Skill_tools></Skill_tools>
   <Footer></Footer>
 </div>
</template>
<script>
import NavbarMenu from "@/components/NavbarMenu.vue";
import Info_detail from "@/components/Info_detail.vue";
import Footer from "./components/footer.vue";
import Skill_tools from "./components/skill_tools.vue";
import Education_info from './components/Education_info.vue';

export default {
  name: "HomeView",
  components: {
    NavbarMenu,
    Info_detail,
    Footer,
    Skill_tools,
    Education_info,
  },
};
</script>
<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  background-color: white;
  color: #2c3e50;
}

nav {
  /* padding: 30px; */
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #42b983;
}
</style>
