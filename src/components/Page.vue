<template>
  <div class="page">
        <header class="page__header">
  
        </header>
        <nav class="page__navbar">

        </nav>
        <main class="page__content">
        </main>
        <footer class="page__footer">

        </footer>
  </div>
</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';

@Options({
  props: {
    msg: String
  }
})
export default class Page extends Vue {
  msg!: string
}
</script>

<style>
    .page__header {
      grid-area: header;
      background: #555456;
      position: sticky;
      top: 0;
    }
    .page__navbar {
      grid-area: navbar;
      background: #123456;
    }
    .page__content {
      grid-area: content;
      background: cornflowerblue;
    }
    .page__footer {
      grid-area: footer;
      background: seagreen;
    }
    .page {
      display: grid;
      min-height: 100%;
      grid-template-columns: 200px 1fr;
      grid-template-rows: 50px 1fr 50px;
      grid-template-areas: 
        "header header"
        "navbar content"
        "footer footer";
    }
</style>
