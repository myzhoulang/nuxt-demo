<template id="product">
  <section>
    <h2> {{ product.name }} </h2>
    <div class="">
      {{ product.desc }}
    </div>
  </section>
</template>

<script type="text/javascript">
  let name = `联想（ThinkPad）黑侠E570 GTX（1NCD）游戏笔记本（i5-7200U 4G 500G+128G SSD GTX950M 2G独显 FHD Win10）`

  let desc = `商品名称：ThinkPad黑侠E570商品编号：3541223商品毛重：3.4kg商品产地：中国大陆系统：Windows 10厚度：20.0mm以上内存容量：4G分辨率：全高清屏（1920×1080）显卡型号：GTX950M待机时长：小于5小时处理器：Intel i5低功耗版特性：其他显卡类别：入门级游戏独立显卡裸机重量：2-2.5kg硬盘容量：128G+500G显存容量：2G·`

  export default {
    data () {
      return {
        product: {
          id: 1,
          name: name,
          desc: desc
        }
      }
    }
  }
</script>
