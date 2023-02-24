<template>
  <div id="app">
    <div>This is the consuming project</div>
    <hr>
    <div>
      Straight from the library 
      <MyButton />
    </div>
    <hr>
    <div>More of the consuming project</div>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import {MyButton} from "vue-cli-comp-lib";

@Component({
  components: { MyButton },
})
export default class App extends Vue {}
</script>

<style lang="scss">
@import "~vue-cli-comp-lib/dist/my-comp-lib.css";
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
