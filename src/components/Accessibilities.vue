<template>
  <section
    id="accessibilities-section"
    class="accessibilities-section section"
    ref="accesibilities"
  >
    <div class="tw-container">
      <div class="tw-flex">
        <div class="tw-w-full">
          <div class="tw-text-center tw-py-10">
            <transition name="fade"
              ><a href="#" class="access-button" v-if="showP"
                ><span>Gửi lời chúc</span></a
              ></transition
            >
            <transition name="fade"
              ><a href="#" class="access-button" v-if="showP"><span>Mừng cưới</span></a></transition
            >
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.accessibilities-section {
  background: url('https://linhda0611.iwedding.info/templates/template15/images/bg.png');
  .access-button {
    display: inline-block;
    text-align: center;
    padding: 12px 20px;
    min-width: 220px;
    margin: 10px 5px 0;
    text-transform: uppercase;
    background-color: #c89d9c;
    border-radius: 0;
    span {
      display: flex;
      align-items: center;
      justify-content: center;
      font-size: 16.5px;
      color: #fff;
      font-weight: 600;
      font-family: 'Comfortaa', sans-serif;
    }
  }
}


</style>

<script lang="ts" setup>
import { ref, onMounted, onUnmounted } from 'vue';

const accesibilities = ref<HTMLElement | null>(null);
const showP = ref<boolean>(false);

const scrolling = async () => {
  if (
    accesibilities.value &&
    accesibilities.value.getBoundingClientRect().top < window.innerHeight &&
    accesibilities.value.getBoundingClientRect().bottom >= 0
  ) {
    showP.value = true;
  } 
};

onMounted(() => {
  window.addEventListener('scroll', scrolling);
});

onUnmounted(() => {
  window.removeEventListener('scroll', scrolling);
});
</script>
