<script lang="ts">
  import Router from "svelte-spa-router";
  // @ts-ignore
  import routes from "virtual:generated-pages-svelte";
  import "./tailwind.css";
</script>

<div class="latar w-full min-h-screen">
  <Router {routes} />
</div>

<style>
  .latar {
    background: url("../latar.jpg") center center no-repeat fixed;
    background-size: cover;
  }
  :global(*) {
    word-wrap: break-word;
  }
  /* chrome extension */
  :global(body) {
    width: 350px;
    font-size: 16px;
  }
</style>
