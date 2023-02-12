<script lang="ts">
  import { cdate } from 'cdate';
  import type { PageData } from './$types';
  import NavHeader from '$lib/components/nav-header.svelte';

  let showAllNews = false;
  export let data: PageData;
</script>

<NavHeader
  targets={[
    { label: '作品', id: '#works' },
    { label: 'ニュース', id: '#news' },
    { label: 'チーム', id: '#about' },
    { label: '連絡先', id: '#contact' },
  ]}
/>

{data.dictionary['games.necromance.title']['ja']}

{#each data.news as item, index}
  {#if showAllNews || index < 3}
    <p>
      {item.title}<br />
      {cdate(item.date).format('YYYY-MM-DD')}<br />
      {item.link}<br />
    </p>
  {/if}
{/each}
<button on:click={() => (showAllNews = !showAllNews)}
  >{showAllNews ? '最新のお知らせのみ表示' : 'さらにお知らせを表示'}</button
>
