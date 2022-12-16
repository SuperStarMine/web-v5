<script lang="ts">
  import type { LayoutData } from './$types';

  export let data: LayoutData;
</script>

<slot />

<style lang="stylus">
  :global(html, body)
    width 100%
    height 100%
    margin 0
</style>
