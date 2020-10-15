<template>
  <Page msg="Welcome to Your Vue.js + TypeScript App"/>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import Page from './components/Page.vue';

@Options({
  components: {
    Page
  },
})
export default class App extends Vue {}
</script>

<style>
#app {
  height: 100%;
  width: 100%;
}
</style>
