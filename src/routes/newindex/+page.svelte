<script lang="ts">
  import { cdate } from 'cdate';
  import type { PageData } from './$types';
  import NavHeader from '$lib/components/nav-header.svelte';
  import SlideHero from '$lib/components/slide-hero.svelte';

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

<SlideHero
  items={[
    {
      id: 'necromance',
      color: '#F7931F',
      title: 'れーぞく！ネクロマンスちゃん',
      subtitle: 'れーぞく全方位シューティングゲーム',
      description: '説明文ここに',
      buttons: [{ label: 'ティザーサイトへ', url: '#' }],
    },
    {
      id: 'necromance',
      color: '#F7931F',
      title: 'れーぞく！ネクロマンスちゃん',
      subtitle: 'れーぞく全方位シューティングゲーム',
      description: '説明文ここに',
      buttons: [{ label: 'ティザーサイトへ', url: '#' }],
    },
    {
      id: 'necromance',
      color: '#F7931F',
      title: 'れーぞく！ネクロマンスちゃん',
      subtitle: 'れーぞく全方位シューティングゲーム',
      description: '説明文ここに',
      buttons: [{ label: 'ティザーサイトへ', url: '#' }],
    },
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
