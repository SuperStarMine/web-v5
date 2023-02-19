<script lang="ts">
  import '@splidejs/svelte-splide/css';
  import { Splide, SplideSlide } from '@splidejs/svelte-splide';

  export let items: {
    id: string;
    color: string;
    title: string;
    subtitle: string;
    description: string;
    buttons: { label: string; url: string }[];
  }[];
</script>

<div class="hero">
  <Splide
    aria-label="ゲーム一覧"
    options={{
      type: 'loop',
      perPage: 1,
      lazyLoad: 'nearby',
      arrows: false,
      pagination: false,
    }}
  >
    {#each items as item}
      <SplideSlide>
        <div class="slide">
          <div class="content">
            <h3 class="subtitle">{item.subtitle}</h3>
            <h2 class="title">{item.title}</h2>
            <div class="description">{item.description}</div>
            <div class="buttons">
              {#each item.buttons as button}
                <a href={button.url}>{button.label}</a>
              {/each}
            </div>
          </div>
          <img
            width="1920"
            height="1080"
            src="https://dummyimage.com/1920x1080/77ff77.png"
            alt="Slide 1"
          />
        </div>
      </SplideSlide>
    {/each}
  </Splide>
</div>

<style lang="stylus">
  .slide
    aspect-ratio 2/1
    img
      width 100%
      height 100%
      object-fit cover
  .content
    position absolute
    bottom 0
    left 0
    padding 5%
</style>
