<template>
  <footer class="site-footer  tw-relative">
      <div class="tw-text-3xl md:tw-text-5xl text">Thank you</div>
  </footer>
</template>

<style lang="scss" scoped>
.site-footer {
  background: url('https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_7088-min.jpg')
    center bottom/100% no-repeat local;
    text-align: center;
    height:100vh;
    display:flex;
    align-items:center;
    justify-content: center;
        background-size: cover;
        @media(max-width: 991px) {
        height:50vh;
      }
    .text {
      font-family: 'Dancing Script';
      font-size: 72px;
      line-height: 1.8em;
      margin: 57.6px 0;
      @media only screen and (max-width: 991px) {
        font-size: 52px;
      }
    }
}
</style>
