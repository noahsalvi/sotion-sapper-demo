<script context="module" lang="ts">
  import { sotion } from "sotion";

  export async function preload() {
    sotion.setScope("765b1258c01c4c8caae4120790e4805a").setFetch(this.fetch);
  }
</script>

<script lang="ts">
  export let segment: string;
  segment;
</script>

<div>
  <slot />
</div>

<style>
  div {
    padding: 0 40px;
    max-width: 900px;
    margin: 0 auto;
  }
</style>
