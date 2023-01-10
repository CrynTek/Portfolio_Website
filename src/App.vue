<template>
  <NavbarMenu></NavbarMenu>
  <Info_detail></Info_detail>
  <Education_info></Education_info>
  <Skill_tools></Skill_tools>
  <WorkShop></WorkShop>
  <footer></footer>
</template>
<script>
import NavbarMenu from "@/components/NavbarMenu.vue";
import Info_detail from "@/components/Info_detail.vue";
import Footer from "./components/footer.vue";
import Skill_tools from "./components/skill_tools.vue";
import WorkShop from "./components/WorkShop.vue";
import Education_info from './components/Education_info.vue';
export default {
  name: "HomeView",
  components: {
    NavbarMenu,
    Info_detail,
    Footer,
    Skill_tools,
    WorkShop,
    Education_info,
  },
};
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
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
