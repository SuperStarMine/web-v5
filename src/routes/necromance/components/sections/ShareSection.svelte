<script>
  import Minicromance from '../../img/mini_necromance.png';
  import ShareText from '../../img/please_share_text.png';
</script>

<div class="share-section">
  <div class="share-section__dialogue">
    <img class="share-section__mini-necromance" src={Minicromance} alt="ミニネクロマンスちゃん" />
    <img class="share-section__text" src={ShareText} alt="シェアしなさいよね！" />
  </div>
  <div class="share-section__share-buttons">
    <a
      class="share-section__button--twitter"
      href="https://twitter.com/intent/tweet?text=%E3%82%8C%E3%83%BC%E3%81%9E%E3%81%8F%E5%85%A8%E6%96%B9%E4%BD%8DSTG%E3%80%8E%E3%82%8C%E3%83%BC%E3%81%9E%E3%81%8F%EF%BC%81%E3%83%8D%E3%82%AF%E3%83%AD%E3%83%9E%E3%83%B3%E3%82%B9%E3%81%A1%E3%82%83%E3%82%93%E3%80%8F%E5%85%AC%E5%BC%8F%E3%82%B5%E3%82%A4%E3%83%88%20https%3A%2F%2Fsuperstarmine.com%2Fnecromance%2F%20%23%E3%81%9E%E3%81%8F%E3%83%AD%E3%83%9E%20%23%E3%82%8C%E3%83%BC%E3%81%9E%E3%81%8F%E3%83%8D%E3%82%AF%E3%83%AD%E3%83%9E%E3%83%B3%E3%82%B9%E3%81%A1%E3%82%83%E3%82%93%20%40necromance_chan%E3%82%88%E3%82%8A%20"
    >
      <svg style="width:24px;height:24px" viewBox="0 0 24 24">
        <path
          fill="currentColor"
          d="M22.46,6C21.69,6.35 20.86,6.58 20,6.69C20.88,6.16 21.56,5.32 21.88,4.31C21.05,4.81 20.13,5.16 19.16,5.36C18.37,4.5 17.26,4 16,4C13.65,4 11.73,5.92 11.73,8.29C11.73,8.63 11.77,8.96 11.84,9.27C8.28,9.09 5.11,7.38 3,4.79C2.63,5.42 2.42,6.16 2.42,6.94C2.42,8.43 3.17,9.75 4.33,10.5C3.62,10.5 2.96,10.3 2.38,10C2.38,10 2.38,10 2.38,10.03C2.38,12.11 3.86,13.85 5.82,14.24C5.46,14.34 5.08,14.39 4.69,14.39C4.42,14.39 4.15,14.36 3.89,14.31C4.43,16 6,17.26 7.89,17.29C6.43,18.45 4.58,19.13 2.56,19.13C2.22,19.13 1.88,19.11 1.54,19.07C3.44,20.29 5.7,21 8.12,21C16,21 20.33,14.46 20.33,8.79C20.33,8.6 20.33,8.42 20.32,8.23C21.16,7.63 21.88,6.87 22.46,6Z"
        />
      </svg>
    </a>
    <a
      class="share-section__button--facebook"
      href="https://www.facebook.com/sharer/sharer.php?kid_directed_site=0&sdk=joey&u=https%3A%2F%2Fsuperstarmine.com%2Fnecromance%2F&display=popup&ref=plugin&src=share_button"
    >
      <svg style="width:24px;height:24px" viewBox="0 0 24 24">
        <path
          fill="currentColor"
          d="M12 2.04C6.5 2.04 2 6.53 2 12.06C2 17.06 5.66 21.21 10.44 21.96V14.96H7.9V12.06H10.44V9.85C10.44 7.34 11.93 5.96 14.22 5.96C15.31 5.96 16.45 6.15 16.45 6.15V8.62H15.19C13.95 8.62 13.56 9.39 13.56 10.18V12.06H16.34L15.89 14.96H13.56V21.96A10 10 0 0 0 22 12.06C22 6.53 17.5 2.04 12 2.04Z"
        />
      </svg>
    </a>
  </div>
</div>

<style lang="stylus">

@import '../../styles/_break.styl'

.share-section
  // FIXME: 実装が正しくないので書き直し
  width: 100%;
  color: #ffffff;
  background-color: #2c2f33;
  display: flex;
  padding: 20px 0;
  gap: 80px;
  justify-content: center;
  flex-wrap: wrap;

  +sm()
    gap: 20px;

  &__dialogue
    display: flex;
    align-items: center;

  &__share-buttons
    display: flex;
    align-items: center;
    gap: 50px;

  &__mini-necromance
    display: inline-block;
    max-height: 100px;
    margin-right: 30px;

    +sm()
      margin-right: 10px;

  $button
    display: inline-block;
    padding: 16px;
    border: 2px solid #fff;
    cursor: pointer;

  &__button
    @extends $button;

    &--twitter
      @extends $button;
      background-color: #1da1f2;

    &--facebook
      @extends $button;
      background-color: #0076fb;
</style>
