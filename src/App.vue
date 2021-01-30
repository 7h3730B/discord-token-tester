<template>
  <Header
    GithubLink="https://github.com/7h3730B/discord-token-tester/"
    title="discord-token-tester"
  />
  <TokenChecker msg="Input your token below" />
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";
import TokenChecker from "./components/TokenChecker.vue";
import Header from "./components/Header.vue";

@Options({
  components: {
    TokenChecker,
    Header
  }
})
export default class App extends Vue {}
</script>

<style lang="scss">
body {
  font-family: "Source Code Pro", monospace, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: purple;
}
#app {
  position: fixed;
  left: 0;
  width: calc(100% - 40px);
  height: 100%;
  background-color: white;
  margin-top: 30px;
  padding: 20px;
}
</style>
