<script lang="ts">
  import NavHeader from '$lib/components/nav-header.svelte';
  import SlideHero from '$lib/components/slide-hero.svelte';
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
