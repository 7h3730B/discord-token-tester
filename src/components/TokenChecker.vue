<template>
  <div class="TokenChecker">
    <p>{{ msg }}</p>
    <input type="text" />
  </div>
</template>

<script lang="ts">
import { Options, Vue } from "vue-class-component";

@Options({
  props: {
    msg: String
  }
})
export default class TokenChecker extends Vue {
  msg!: string;
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.TokenChecker {
  background-color: rgb(0, 153, 255);
  width: 100%;
  display: flex;
  flex-direction: column;
  justify-content: center;
}
</style>
