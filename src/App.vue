<template>
  <div id="app">
    <app-header profiletitle="Profile Card"></app-header>

    <main class="main">
      <app-side-bar sidebartitle="SideBar"></app-side-bar>
      <app-content
        @submit="update($event)"
        contenttitle="Content"
      ></app-content>
      <app-aside asidetitle="Aside"></app-aside>
    </main>
    <app-footer></app-footer>
  </div>
</template>

<script>
import AppHeader from "./components/AppHeader";
import AppContent from "./components/AppContent";
import AppAside from "./components/AppAside";
import AppFooter from "./components/AppFooter";
import AppSideBar from "./components/AppSideBar";

export default {
  name: "App",
  components: {
    AppHeader,
    AppContent,
    AppAside,
    AppFooter,
    AppSideBar,
  },
};
</script>

<style lang="scss">
@import url("./css/global.css");
#app {
  display: flex;
  flex-direction: column;
  height: 100vh;
  border: 5px dashed #000000;
  & .main {
    display: flex;
    flex-direction: row;
    flex-grow: 1;
    border: 5px dashed #8a2be2;
  }
}
</style>
