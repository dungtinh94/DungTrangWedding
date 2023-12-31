<template>
  <section id="album" class="wedding-album">
    <div class="lg:tw-container">
      <div class="sm:tw-block tw-flex tw-px-3.5">
        <div class="tw-w-3/4 tw-mx-auto">
          <div class="title tw-font-comfortaa tw-mb-8">
            <h2>Album Hình Cưới</h2>
            <p>
              Được ai đó yêu sâu sắc sẽ mang lại cho bạn sức mạnh, trong khi yêu ai đó sâu sắc sẽ
              cho bạn dũng khí.
            </p>
          </div>
        </div>
      </div>
      <div class="tw-columns-3xs">
        <a-image-preview-group>
          <a-image class="tw-mb-4" v-for="image in images" :src="image.url" alt=""/>
        </a-image-preview-group>
        
      </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>
.wedding-album {
  padding: 100px 0;
  text-align: center;
  .title {
    position: relative;
    text-align: center;
    padding-top: 70px;
    &::after {
      content: '';
      background: url('https://linhda0611.iwedding.info/templates/template15/images/sec-title-flower.png')
        center center/cover no-repeat local;
      width: 126px;
      height: 59px;
      position: absolute;
      top: 0;
      left: 50%;
      transform: translateX(-50%);
    }
    h2 {
      font-family: 'Dancing Script';
      font-size: 36px;
      margin-bottom: 14px;
      font-weight: 700;
    }
    p {
      font-size: 1.05rem;
    }
  }
  .album-button {
    text-align: center;
    display: flex;
    align-items: center;
    justify-content: center;
    background-color: #c89d9c;
    color: #fff;
    line-height: 17.6px;
    width:200px;
    height:38px;
    font-weight: 600;
    border: 0;
    border-radius: 4px;
    margin-top: 20px;
    margin-bottom: 52px;
    &:hover {
      background-color: #b58887;
      color: #fff;
      text-decoration: none;
    }
  }
  .gallery-container {
    gap: 15px;
    margin: 0 -7.5px;
  }
}
</style>

<script lang="ts" setup>
import {ref} from "vue"
interface Image {
  id: number;
  url: string;
}

const images:Image[] = [
  {
    id: 1,
    url: 'https://edtexco-x360-dev.s3.amazonaws.com/dev/images/tuan/THK_5991-min.jpg',
  },
  {
    id: 2,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_5992-min.jpg',
  },
  {
    id: 3,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_5998-min.jpg',
  },
  {
    id: 4,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6018-min.jpg',
  },
  {
    id: 5,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6069-min.jpg',
  },
  {
    id: 6,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6118-min.jpg',
  },
  {
    id: 7,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6208-min.jpg',
  },
  {
    id: 8,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6435-min.jpg',
  },
  {
    id: 9,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6490-min.jpg',
  },
  {
    id: 10,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6544-min.jpg',
  },
  {
    id: 11,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6562-min.jpg',
  },


   {
    id: 12,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6579-min.jpg',
  },
  {
    id: 13,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6596-min.jpg',
  },
  {
    id: 14,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6611-min.jpg',
  },
  {
    id: 15,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6897-min.jpg',
  },
  {
    id: 16,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6901-min.jpg',
  },
  {
    id: 17,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6929-min.jpg',
  },
  {
    id: 18,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6946-min.jpg',
  },
  {
    id: 19,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6971-min.jpg',
  },
  {
    id: 20,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6982_%282%29-min.jpg',
  },
  {
    id: 21,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_7031-min.jpg',
  },
  {
    id: 22,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_7051-min.jpg',
  },
    {
    id: 23,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_7066-min.jpg',
  },
  {
    id: 24,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_7073-min.jpg',
  },
  {
    id: 25,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_7093-min.jpg',
  },
  {
    id: 26,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_7222-min.jpg',
  },
  {
    id: 27,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_7231-min.jpg',
  },
  {
    id: 28,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_7243-min.jpg',
  },

      {
    id: 29,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_7245-min.jpg',
  },
  {
    id: 30,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_7301-min.jpg',
  },
  {
    id: 31,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_7325-min.jpg',
  },
  {
    id: 32,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_7332-min.jpg',
  },
  {
    id: 33,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_7336-min.jpg',
  },
];

const imagesList=ref<any>([  {
    id: 1,
    url: 'https://edtexco-x360-dev.s3.amazonaws.com/dev/images/tuan/THK_5991-min.jpg',
  },
  {
    id: 2,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_5992-min.jpg',
  },
  {
    id: 3,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_5998-min.jpg',
  },
  {
    id: 4,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6018-min.jpg',
  },
  {
    id: 5,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6069-min.jpg',
  },
  {
    id: 6,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6118-min.jpg',
  },
  {
    id: 7,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6208-min.jpg',
  },
  {
    id: 8,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6435-min.jpg',
  },
  {
    id: 9,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6490-min.jpg',
  },
  {
    id: 10,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6544-min.jpg',
  },
  {
    id: 11,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6562-min.jpg',
  },


   {
    id: 12,
    url: 'https://edtexco-x360-dev.s3.ap-southeast-1.amazonaws.com/dev/images/tuan/THK_6579-min.jpg',
  },]);

const handleShowMore =()=>{
  console.log('ádasd')
}
</script>
