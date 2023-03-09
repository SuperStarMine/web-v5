<script lang="ts">
  import type { PageData } from './$types';
  import './global.stylus';

  export let data: PageData;

  // import Cframe from "$lib/components/deprecated/common-frame.svelte";
  import Nheader from "$lib/components/deprecated/nav-header.svelte";
  // import Static from "$lib/components/deprecated/static-content.svelte";
  // import Dlist from "$lib/components/deprecated/date-list.svelte";
  // import HeroS from "$lib/components/deprecated/slide-hero-swiper.svelte";
  // import Desc from "$lib/components/deprecated/slide-description.svelte";
  // import Footer from "$lib/components/deprecated/footer.svelte";
  // import Cards from "$lib/components/deprecated/cards.svelte";
</script>


<Nheader/>
<!-- <main style="--transitionDuration: 500ms;--standardWidth: {$sync.standardWidth}vw"> -->
<main style="--transitionDuration: 500ms;--standardWidth: 80vw">
  <!-- {#each settings as {title, subtitle, themeColor, sectionType, contents, id, pairId}}
    {#if sectionType == "slideHero"}
      <HeroS contents={contents || settings.find(v => v.pairId == pairId && v.isParent).contents} {globalSettings} {pairId} standardWidth={$sync.standardWidth}/>
    {:else if sectionType == "slideDesc"}
      <Desc {contents} {globalSettings} {pairId} standardWidth={$sync.standardWidth}/>
    {:else if sectionType == "footer"}
      <Footer {contents}/>
    {:else if sectionType != "navHeader"}
      <Cframe {id} {title} {subtitle} {themeColor}>
        {#if sectionType == "static"}
          <Static {contents} {globalSettings} standardWidth={$sync.standardWidth}/>
        {:else if sectionType == "dateList"}
          <Dlist {contents}/>
        {:else if sectionType == "cards"}
          <Cards {contents} {globalSettings} standardWidth={$sync.standardWidth}/>
        {/if}
      </Cframe>
    {/if}
  {/each} -->
</main>
