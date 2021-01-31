<template>
  <header>
    <div class="header">
      <h3 class="child">{{ title }}</h3>
      <a class="child" target="_blank" :href="GithubLink"> Github </a>
    </div>
  </header>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  props: {
    GithubLink: {
      required: true,
      type: String
    },
    title: {
      required: true,
      type: String
    }
  }
})
export default class Header extends Vue {}
</script>

<style scoped>
.header {
  position: fixed;
  left: 0;
  top: 0;
  width: 100%;
  background-color: black;
  display: flex;
  flex-wrap: column;
  justify-content: space-between;
  text-align: center;
  padding: 3px;
  color: white;
}
.child {
  margin: 5px 20px 5px 20px;
}
a:visited,
a {
  transition: 0.25s color ease-out;
  color: rgb(163, 163, 163);
}
a:hover {
  color: white;
}
</style>
