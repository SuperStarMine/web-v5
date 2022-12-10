<script lang="ts">
  import NavHeader from '$lib/components/nav-header.svelte';
</script>

<NavHeader
  targets={[
    { label: '作品', id: '#works' },
    { label: 'ニュース', id: '#news' },
    { label: 'チーム', id: '#about' },
    { label: '連絡先', id: '#contact' },
  ]}
/>


<style lang="stylus">
  :global(body)
    background-color #e5e5e5
</style>
