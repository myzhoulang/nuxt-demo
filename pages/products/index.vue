<template id="products">
  <section>
    <h2>商品列表页面</h2>

    <ul>
      <li v-for="product in products">
        <span>{{ product.name }}</span>
        <time>{{ product.time }}</time>
      </li>
    </ul>
  </section>
</template>

<script type="text/javascript">
  let axios = require('axios')
  let url = `https://www.ele.me/restapi/shopping/restaurants?extras%5B%5D=activities&geohash=wtmkps3fh90&latitude=30.25807&limit=24&longitude=120.215&offset=0&terminal=web`

  export default {
    layout: 'products',
    // 异步数据获取
    async asyncData (context) {
      try {
        const { data } = await axios.get(url)
        console.log(data)
        return {
          products: data
        }
      } catch (err) {
        console.log(err)
      }
    }
  }
</script>
